<template> 
<div id="navBAR_DOCENTE">
    <ul> 
        <li> <a href="login_adm.html"> Login </a> </li>
        <li> <a href="cadastroDOCENTE.html"> Cadastro </a></li>
    </ul>
</div>

<div id="login_adm">  
    <div id="outro">
    
        <h1> Insira seus dados para o login: </h1>

        <form> 
            <label> Insira seu número do SIAPE:<br>  <input type="text" id="siape_docente" name="siape_docente"/></label><br><br> 
            <label> Insira sua senha: <br> <input type="password" id="senha_docente" name="senha_docente" minlength="8" required /></label><br><br> 
        </form>

    </div>
</div>
</template>