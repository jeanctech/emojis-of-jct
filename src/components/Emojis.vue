<script setup>
import { ref } from 'vue'

const showCopied = ref(false)

const copyEmoji = async (emoji) => {
  try {
    await navigator.clipboard.writeText(emoji)
    
    showCopied.value = true
    setTimeout(() => {
      showCopied.value = false
    }, 2000)
    
  } catch (err) {
    console.log('Error al copiar:', err)
  }
}

const emojis = ['😀',
'😃',
'😄',
'😁',
'😆',
'😅',
'🤣',
'😂',
'🙂',
'🙃']
</script>

<template>
  <div>
    <!-- Tus emojis clickeables -->
    <span 
      v-for="emoji in emojis" 
      :key="emoji"
      @click="copyEmoji(emoji)"
      class="emoji-item"
    >
      {{ emoji }}
    </span>
    
    <!-- Mensaje de copiado -->
    <div v-if="showCopied" class="toast">
      ✨ ¡Copiado!
    </div>
  </div>
</template>

<style>
.emoji-item {
  cursor: pointer;
  padding: 8px;
  border-radius: 4px;
  display: inline-block;
  transition: background-color 0.2s;
}

.emoji-item:hover {
  background-color: #f0f0f0;
}

.toast {
  position: fixed;
  top: 20px;
  right: 20px;
  background: #4CAF50;
  color: white;
  padding: 10px 20px;
  border-radius: 4px;
}
</style>