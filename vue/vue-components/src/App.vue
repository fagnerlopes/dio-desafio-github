<template>
  <div id="app">
    <p>Recomendado - Component separado em arquivo</p>
    <ButtonVue></ButtonVue> 
    <p>Componente Global - Template passado no construtor como uma <strong>string</strong></p>
    <ButtonString></ButtonString> 

    <p> Componente Global - Template passado no construtor como <strong>Template Literals</strong></p>
    <ButtonTemplateString></ButtonTemplateString>
    <p> Componente Global - Template injetado <strong>diretamente no Index.html com a flag x-template</strong></p>
    <ButtonXTemplate></ButtonXTemplate>
    <p> Componente Global - Template injetado <strong>ao instanciar o componente com a flag inline-template</strong></p>
    <ButtonInlineTemplate inline-template>
      <button @click="click">
        Click ButtonInlineTemplate {{ count }} times
      </button>
    </ButtonInlineTemplate>
    <p> Componente Global - Template injetado via método render <strong>que é passado como 3 parâmetro do contrutor</strong></p>
    <ButtonRender></ButtonRender>
    <p> Componente Global - Template injetado via método render <strong>que é passado como 3 parâmetro do contrutor e usando sintaxe JSX</strong></p>
    <ButtonJSX/>
  </div>
</template>

<script>
import ButtonVue from './ButtonVue.vue'

export default {
  name: 'App',
  components: {
    ButtonVue,
  }
}
</script>

<style>
#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  gap: 5px;
}
</style>
