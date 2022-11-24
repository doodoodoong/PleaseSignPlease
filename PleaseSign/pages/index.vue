<template>
  <div>
    <p class="text-black text-3xl text-center">편리한 회의록 서명</p>
    <p class="text-black text-xl text-center">
      아래에 회의록 파일을 등록해주세요
    </p>
    <div>
      <v-file-input color="black" accept=".pdf" label="Your PDF file input">
      </v-file-input>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
