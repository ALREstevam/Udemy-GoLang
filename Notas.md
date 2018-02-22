
# Udemy - GoLang

# Introdução
## É uma linguagem...
* Compilada
* Fortemente tipada
* Robusta 
* Criada pela Google para resolver problemas que tinham com C/C++
* Focada no paralelismo / uso de multicore
* Não é funcional (mas aplica alguns dos conceitos de programação funcional)
* Não é orientada a objeto (mas usa alguns conceitos, como interface)
	* Polimorfismo, métodos, pacotes, public, private
* Onde as funções podem ser tratadas como parâmetros e variáveis
* Onde as funções podem retornar múltiplos valores
* Criada após o mundo multicore (uma das poucas)
* Onde a própria engine ajuda nos testes unitários e de cobertura (embutido na linguagem)
* Ser server (Apache, Ngnx) consegue processar requisições HTTP, a própria linguagem tem recursos para lidar com isso de forma robusta e pronta para a produção
* De código aberto/ livre

> **Linguagem fortemente tipada**, resumindo, seria aquela em que os objetos/variáveis tem um tipo bem definido e que precisa ser informado no momento de sua declaração.
(https://www.devmedia.com.br/forum/linguagem-fortemente-tipada/425615)

## Se baseia em
* Ter uma linguagem mínima
* Não ter muitas formas de fazer a mesma coisa
* Simplicidade e minimalismo
* Concorrência como parte da linguagem

## Resolve problemas
* Complexidade da concorrência e paralelismo (concorrência pode ativar o paralelismo)
* Se baseando em C/C++ pretende resolver o problema da complexidade da linguagem sem perder o desempenho dessas linguagens
* 


> **Obs.:** Concorrência não é paralelismo!


# História da linguagem

* Foi apresentada em novembro de 2009
* Criada pelos engenheiros
	* Robert Griesemer
	* Rob Pike
	* Ken Thompson

* Go 1.0: Março de 2012

## Pontos de partida

* Desenvolvedores que precisavam de muito desempenho se frustaravam com linguagens como C++

* C++ é rápido, porém
	* Demora muito para compilar
	* Algumas coisas são muito complexas de se fazer
	* Existem problemas de compilação
	* Existem muitas formas de resolver o mesmo problema
	* Muitas formas de fazer a mesma coisa
	* Manuais grandes e complexos

**Algumas alternativas:**

* Python e outras linguagens interpretadas: muito lento
* Java e linguagens que dependem de uma VM: a máquina virtual é um gargalo

**Com isso em mente, na Google foi criada a linguagem Go, a empresa pretendia que a linguagem fosse:**
* Limpa
* Pequena
* Compilada (muito mais eficiente que linguagens interpretadas)
* Recursos de linguagen modernas
* Tempo de compilação baixo (é mais rápido que a interpretação em linguagens interpretadas)

## Princípios
* Simples
* Segura (quanto a memória (garbage collector))
* Fácil legibilidade (fácil de escrever e de manter)
* Mínima (uma única forma de escrever um determinado tipo de código)
	* Só um laço
	* Operadores unários (prefixado (++x) / pósfixado (x++)), go só tem uma
	* Consolidaram o que já existia (papers e outras linguagens)

## História das linguagens
* Go foi baseado em:
	* Algo60
	* Pascal
	* C
	* Modula, Modula-2
	* Oberon, Oberon-2
	* Smalltalk (influência OO)
	* NewSquik (influência da concorrência)(projeto do Rob Pike) (evita o uso de callbacks)

> **Callback** é uma função que é usada como "callback". Ela é tipicamente passada como argumento de outra função e/ou chamada quando um evento for acontecido, ou quando uma parte de código receber uma resposta de que estava à espera.
> Isto é muito comum em javascript lado cliente e servidor (NodeJS) mas não só. A função callback é muitas vezes assíncrona na medida em que é chamada como consequência de outro código que esta a correr no background. A grande vantagem é que assim o computador pode ir processando outros processos enquanto a resposta não chega e não precisa assim de parar tudo à espera dessa resposta.
> (https://pt.stackoverflow.com/questions/27177/o-que-é-callback)

* Quanto a sintaxe
	* ***C-like, Oberon structure***


> **Linguagens C-like:**  C++, Java, Objective-C, C#, Javascript


* É baseado em conceitos de linguagens antigas mas usa conceitos de linguagens atuais, como:
	* Orientação a Objetos
	* Generics
	* Linguagens dinâmicamente tipadas

> **Crítica ao modelo OO:** *programas complexos em OO é a nova versão do "spaghetti code"* (códigos cheios de `goto` em 1970)
> * Não é um paradigma simples de ser aplicado
> * Não força o desenvolvedor a criar código manutenível (dificuldade de manter o código organizado)

Resultdo no Go:
* Não foram trazidos da OO conceitos como:
	* Classes
	* Herança
	* ...
* E foram trazidos
	* Polimorfismo
	* Interfaces
	* Métodos

## Configuração do ambiente
1. Download e instalação do Go: https://golang.org/dl/
2. Download e instalação do VisualStudioCode: https://code.visualstudio.com/download
3. No VS Code adicionar as extensões:
	* Go for Visual Studio Code
	* Code Runner

4. Criar o código de teste `teste.go`
5. No topo da tela, o VS Code pedirá para instalar alguns complementos, clicar em install
6. Começar a escrever o código, mais avisos aparecerão, instalar
7. Usar o atalho `ctrl+alt+n` para executar o código com o Code Runner
* `ctrl+alt+m` para o código em execução
* Na linha de comando: `cd <diretório do arquivo go>`, `go run <filename>.go`
