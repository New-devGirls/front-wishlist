<template>
    <div class="fundo ">
        <div class="login">
            <h1>Login</h1>
            <br><br>
            <input type="text" placeholder="Email">
            <br><br>
            <input type="password" placeholder="Senha">
            <br><br>
            <button>Entrar</button>
        </div>
    </div>
    
</template>

<script>
export default {
    setup() {
        
    },
}
</script>

<style scoped>

.fundo{
    background-image: repeating-linear-gradient(45deg, #90B3FE, #FF857E);
    height: 100vh;
    width: 100vw;
    overflow-y: hidden;
}
.login{
    background-color: rgba(92, 41, 41, 0.5);
    border-radius: 10px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    padding: 70px;
    color: #fff;
}
input{
    padding: 20px;
    border: none;
    outline: none;
    font-size: 15px;
    border-radius: 10px;
}
button{
    background-color: dodgerblue;
    border: none;
    padding: 15px;
    width: 100%;
    border-radius: 10px;
    color: white;
}
button:hover{
    background-color: deepskyblue;
    cursor: pointer;
}
@media (max-width: 858px){
    .login{
        border-radius: 10px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        padding: 45px;
        color: #fff;
    }
    input{
        padding: 10px;
        border: none;
        outline: none;
        font-size: 15px;
        border-radius: 10px;
    }
    button{
        background-color: dodgerblue;
        border: none;
        padding: 10px;
        width: 100%;
        border-radius: 10px;
        color: white;
    }
}
</style>