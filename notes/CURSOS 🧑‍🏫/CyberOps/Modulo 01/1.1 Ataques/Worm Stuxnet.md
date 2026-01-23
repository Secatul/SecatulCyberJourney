Entenda aqui: https://www.malwarebytes.com/pt-br/stuxnet

O **Stuxnet** é um programa malicioso muito sofisticado que foi descoberto em 2010. Ele é considerado a primeira "arma cibernética" da história porque foi especificamente criado para destruir equipamentos físicos, não apenas roubar dados ou danificar softwares.

O Stuxnet foi desenvolvido por agências de inteligência dos EUA e Israel (CIA, NSA e Mossad) para sabotagem o programa nuclear do Irã, especificamente as centrífugas de enriquecimento de urânio na Usina de Natanz. Essas centrífugas são máquinas que giram a altíssimas velocidades para separar isótopos de urânio, um processo essencial para produzir material nuclear.

### Como funciona
1. **Entrada pela USB**: Como a usina nuclear era "isolada do ar" (não conectada à internet), o Stuxnet foi inserido através de um pen drive infectado, provavelmente por um funcionário ou contratado da instalação.
2. **Procurava o Alvo Específico**: Depois de infectar computadores, o worm procurava por um software específico chamado Siemens Step 7, usado para controlar as centrífugas.
3. **O Sabotage**: Uma vez encontrado o alvo, o Stuxnet alterava as instruções enviadas às centrífugas, fazendo-as girar de forma irregular e danificada. Ao mesmo tempo, ele enviava **dados falsos** aos monitores dos engenheiros iranianos, mostrando que tudo estava funcionando normalmente.[](https://www.trellix.com/security-awareness/ransomware/what-is-stuxnet/)​
4. **Resultado**: As centrífugas começavam a se autodestruir lentamente, sem que os operadores percebessem o que estava acontecendo até ser tarde demais.

### Impacto
- Destruiu aproximadamente **1.000 das 5.000 centrífugas** iranianas
- Atrasou o programa nuclear iraniano em **vários anos**
- Infectou mais de 100.000 computadores, mas só causava dano real nos computadores com a configuração específica da usina de Natanz