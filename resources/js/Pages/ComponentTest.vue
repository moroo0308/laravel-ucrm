<script setup>
import GuestLayout from '@/Layouts/GuestLayout.vue';
import InputLabel from '@/Components/InputLabel.vue';
import TextInput from '@/Components/TextInput.vue';

const emitTest = e => console.log(e);

</script>

<template>
  <div>
    <GuestLayout>
      <InputLabel value="件名"></InputLabel>
      <TextInput modelValue="初期値が入ります" @update:modelValue="emitTest">
      </TextInput>
    </GuestLayout>
  </div>
</template>