# Bertoti

# Raul Santos Iglesias - 1460481911069

# Ciclo de vida do desenvolvimento de Softwares (Go2Learning)

## 💻Requisitos

> Funcionais: (Caso de uso)
<br>


São as funcionalidades de um sistema, é o que define o que o sistema fará;

<div align="center">
  
![casoUsoRaulSantosIglesias](https://user-images.githubusercontent.com/51235779/161818806-eef4d81d-6163-466b-a6cf-9ed07888b6dd.jpg)

  
</div>

> Não funcionais: (Heurísticas)

<br>

São todas as necessidades que não podem ser atendidas através de funcionalidades, as qualidades de um sistema;

<div align="center">
	
![image](https://user-images.githubusercontent.com/51235779/161824495-cd155277-4a04-429d-a80d-0c6dacb0096d.png)


</div>  

## 💻Projeto

> Classes 

<div align="center">
  
  ![diagramClassRaul](https://user-images.githubusercontent.com/51235779/161818998-24dda2e6-835d-4877-b9b5-5c9b8c0fb5b8.jpg)


</div>

## 💻Desenvolvimento

> Classes e JAVA
<br>

#### ©  Classe Go2Learning

![image](https://user-images.githubusercontent.com/51235779/161819176-13e93eb3-2705-4bdc-9360-1d44d3085c78.png)


> Código em JAVA

```JAVA


import java.util.LinkedList;
import java.util.List;

public class Go2Learning{

     private List<Integrante> Integrantes= new LinkedList<Integrante>();

     public void cadastrarIntegrante(Integrante Integrante){
          Integrantes.add(Integrante);
     }

     public List<Integrante> buscarIntegrantePorNome(String nome){
           List<Integrante> nomesEncontrados = new LinkedList<Integrante>();
           for(Integrante Integrante:Integrantes){
                if(Integrante.getNome().equals(nome)) nomesEncontrados.add(Integrante);
           }
           return nomesEncontrados;
     }

     public Integrante buscarIntegrantePorMatricula(String matricula){
          for(Integrante Integrante:Integrantes){
               if(Integrante.getMatricula().equals(matricula)) return matricula; 
          }
          return null;
     }

     public List<Integrante> getIntegrantes(){
           return Integrantes;
     }
}
```
<br>
<br>

#### © Classe Pessoa

![image](https://user-images.githubusercontent.com/51235779/161819262-e632c769-b9bc-41d4-80b2-6bf213d94d7a.png)


> Código em JAVA

```JAVA
public class Integrante {
	
	private String nome;
	private String matricula;
	private String tipo;
	
	public Integrante(String nome, String matricula, String tipo) {
		this.nome = nome;
		this.matricula = matricula;
		this.tipo = tipo;
	}

	public String getNome(){
		return nome;
	}
	
	public void setNome(String novoNome){
		nome = novoNome;
	}

	public String getMatricula() {
		return matricula;
	}

	public void setMatricula(String matricula) {
		matricula = novaMatricula;
	}
	
	public String getTipo(){
		return tipo;
	}
	
	public void setTipo(String tipo){
		tipo = novoTipo;
	}

}
```
<br>
<br>

#### © Classe Aula

![image](https://user-images.githubusercontent.com/51235779/161819354-d3a6b74c-fe4d-4be0-91d0-873319216f50.png)


> Código em JAVA

```JAVA
public class Aula{
	
	private String nomeAula;
	private String nomeIntegrante;
	
	public Integrante(String nomeAula, String nomeIntegrante) {
		this.nomeAula = nomeAula;
		this.nomeIntegrante = nomeIntegrante;
	
	}

	public String getNomeAula(){
		return nomeAula;
	}
	
	public void setNomeAula(String novoNomeAula){
		nomeAula = novoNomeAula;
	}

	public String getNomeIntegrante() {
		return nomeIntegrante;
	}

	public void setMatricula(String nomeIntegrante) {
		nomeIntegrante = novoNomeIntegrante;
	}
	
	

}
```

