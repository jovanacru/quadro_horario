<template>
  <div id="navBAR_DOCENTE">
        <ul> 
            <li> <a href=""> Login </a> </li>
            <li> <a href=""> Cadastro</a></li>
        </ul>
    </div>

    <div id="cadastrando_docente">
        <div id="outr"> 

            <h1> Insira seus dados para cadastrar-se: </h1>
            
            <form> 
            <label> Insira seu Nome: <br> <input type="text" id="nome_docente" name="nome_docente"/></label>
            <br><br> 
             
            <label> Insira seu email: <br> <input type="text" id="email_docente" name="email_docente"/></label>
            <br><br> 
              
            <label> Insira seu número do SIAPE:<br>  <input type="text" id="siape_docente" name="siape_docente"/></label>
            <br><br> 
              
            <label> Insira sua senha: <br> <input type="password" v-model="senha_docente" id="senha_docente" name="senha_docente" minlength="4" required /></label>
        <br><br> 
            
            <label> Insira sua senha: <br> <input type="password" v-model="senha2_docente" id="senha2_docente" name="senha2_docente" minlength="4" required /></label>
        <br><br> 

            <form>
                <h3>  Informe se você faz parte da docencia ou administraçaõ:</h3>
                <input TYPE="checkbox" v-model="escolha1" NAME="Docente" VALUE="op1"> Docente
                <input TYPE="checkbox" v-model="escolha2" NAME="Administração" VALUE="op2"> Administração
            </form>
           

            <br><input type="submit" value="Enviar">

            </form>
            </div>
        </div>
</template>

<script>

    import login from './components/login.vue';

    export default {
            name: "submit",
            data() {
              return {
                escolha1: 'Docente',
                escolha2: 'Administração',
                senha2_docente: '',
                senha_docente:''
                  }
            components:{
                login
            }
        }
      }

</script>

<style>

#cadastrando_docente {
   padding: 120px;
   padding-right: 147px;
   display: flex;
   justify-content: center;
   
}

#login_adm {
  padding: 120px;
  padding-right: 147px;
  display: flex;
  justify-content: center;
}

ul {
    list-style-type: none;
    overflow: hidden;
    background-color: #333;
    padding: 9px;
    display: flex;
    justify-content: end;
    margin: 0px;

  }
  
  body{
    margin:0px ;
  }

  #outr {
    justify-content: center;
    display: flex;
    flex-direction: column;
  }
  
  
  li a {
    display: block;
    color: white;
    text-align: center;
    padding: 20px 58px;
    text-decoration: none;
  }
  
  li a:hover {
    background-color: #111;
  }



</style>