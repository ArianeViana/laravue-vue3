<template>
    <div id="container">
        <h1>Loops</h1>
        <div v-for="pessoa in pessoas" v-bind:key="pessoa.id" id="loops">
            <p>Nome:{{ pessoa.nome }} <br>
                Idade: {{ pessoa.idade }} <br></p>

        </div>
    </div>
</template>

<script>
export default {
    name: 'OsLoops',
    data() {
        return {
            pessoas: [
                {
                    id: 1,
                    nome: "Breno Souza",
                    idade: 31
                },
                {
                    id: 2,
                    nome: "Clara Barros",
                    idade: 21
                }, {
                    id: 3,
                    nome: "Maria Lima",
                    idade: 45
                }
            ]
        }
    }
}
</script>

<style scoped>
#container {
    background-color: aqua;
    width: 200px;
}

h1 {
    text-align: center;
    padding-top: 5px;
}

#loops {
    border: 1px solid black;
    text-align: center;
}
</style>