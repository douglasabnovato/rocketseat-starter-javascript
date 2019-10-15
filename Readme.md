# Rocketseat - Starter JavaScript 

## Atualização: 15 de Outubro de 2019 - 12:04
## Criação: 14 de Outubro de 2019
## Prática : @douglasabnovato

## Ferramentas : 

![Git](/images/logo-git.png)
![Github](/images/logo-github.png)
![Javascript](/images/logo-javascript.png)
![VSCode](/images/logo-VSCode.png)
![Rocketseat](/images/logo-rocketseat.png)

### Introdução à Javascript 

#### 1. Introdução 
- interpretar scripts na interface do navegador no ambiente do cliente.
- comunidade javascript.

#### 2. Configuração Ambiente 
- Visual Studio Code
- Console de Desenvolvedor - Google Chrome

#### 3. Variáveis e Dados
- string, inteiro, decimal, boolean, vetor, objeto
- console.log
````
	var nome = "douglas";//string
	var idade = 29;//inteiro
	var peso = 80.5;//decimal
	var humano = true;//boolean
	var alunos = ['douglasabn', 'Roberto', 'Lucas'];//vetor
	var aluno = {//objeto
	    nome: 'douglasabnovato',
	    idade: 29,
	    peso: 84.5,
	    humano: true
	};
	console.log(alunos[1]);
	console.log(aluno.peso);
````

#### 4. Operações Matemáticas

````
	var x = 9, y = 3;
	console.log(x + y);
````

#### 5. Funções
````
	function soma(numero1, numero2){
	    var resultado = numero1 + numero2;
	    return resultado;
	}
	var resultadosoma = soma(1, 2);
	console.log(resultadosoma);
````

#### 6. Condicionais
- if
````
	function qualSexo(sexo){//M ou F
	    if(sexo == 'M'){
	        return 'Masculino';
	    } else if( sexo == 'F') {
	        return 'Feminino'; 
	    } else {
	        return 'Outro';
	    }
	}
	var resultadoSexo = qualSexo('M');
	console.log(resultadoSexo);
````

- switch case
````
	function qualSexo(sexo){//M ou F
	    switch (sexo) {
	        case 'M':
	            return 'Masculino';
	        case 'F':
	            return 'Feminino';
	        default:
	            return 'Outro';
	    }
	}
	var resultadoSexo = qualSexo('F');
	console.log(resultadoSexo);
````

#### 7. Operadores Lógicos
- and/ or/ not
````         
	var sexo = 'M', idade = 23;
	if(sexo === 'M' && idade >=18){
	    console.log('OK');
	}
````

#### 8. Condicional Ternária
- estrutura tradicional if else
````
	var sexo = 'M';
	if (sexo === 'M'){
	    return 'Masculino';
	} else {
	    return 'Feminino';
	}
````
- estrutura ternária
````
	var sexo = 'F';
	var retorno = (sexo === 'M') ? 'Masculino' : 'Feminino';
	console.log(retorno);
````

#### 9. Estruturas de Repetição
- for : exibir no console de 0 a 99 
````
	for (var i = 0; i < 100; i++){
	    console.log(i);
	}
````
- while - quando não há conhecimento de quantas interações serão realizadas
````
	var j = 0;
	while (j<100){
	    console.log(j);
	    j++;
	}
````

#### 10. Intervalo e Timeout
- Intervalo : executa repetidas vezes no intervalo de tempo informado como parâmetro
````
	function exibirAlgo(){
	    console.log('@douglasabnovato');
	}
	setInterval(exibirAlgo, 1000);
````
- Timeout : executa uma vez após o intervalo de tempo informado como parâmetro
````	
	function exibirAlgo(){
		console.log('@douglasabnovato');
	}
	setTimeout(exibirAlgo, 6000);
````

#### Desafio
- arquivo pdf : desafio1-introducao.pdf
- tarefa 1
````
	<script>  
		var endereco = {
		    rua: "Rua dos pinheiros",
		    numero: 1293,
		    bairro: "Centro",
		    cidade: "São Paulo",
		    uf: "SP"
		};
		function montarEndereco(){

		    return 'O usuário mora em ' + endereco.cidade + '/' + endereco.uf 
		            + ', no bairro ' + endereco.bairro + ', na rua ' + endereco.rua 
		            + ' com nº ' + endereco.numero + '.'
		}

		console.log(montarEndereco());

	</script>
````
- tarefa 2
````
	function exibirPares(x, y){
		for(var i = x; i <= y; i++){
		    if(i%2 === 0){
		        console.log(i);
		    } 
		}
	}
	console.log(exibirPares(32,321));
````
- tarefa 3
````
	function temHabilidade(skills, possuiEssaSkill){
	    return skills.indexOf(possuiEssaSkill);
	}

	var skills = [ "Html", "Javascript", "ReactJS", "React  Native"];
	var possuiEssaSkill = "Javascript";

	if(temHabilidade(skills, possuiEssaSkill) != -1){
	    console.log('Possui a habilidade ' + possuiEssaSkill + '.');
	} else {
	    console.log('Não Possui a habilidade ' + possuiEssaSkill + '.');
	}
````

:. De Rocketseat - Starter - Javascript.<br>
Por Diego Fernandes : https://skylab.rocketseat.com.br/node/curso-java-script/group/introducao-java-script/lesson/configurando-ambiente-3