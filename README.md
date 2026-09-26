# 🤖 Projeto II: Robô Patrulha com Desvio de Obstáculos (LEGO MINDSTORMS EV3)

Repositório dedicado à documentação, código e evidências do **Projeto Patrulha**, desenvolvido para a oficina de Programação e Robótica LEGO MINDSTORMS EV3 (STEAM). O objetivo principal foi projetar e programar um robô autônomo capaz de realizar um percurso utilizando o seguimento de linha, identificar obstáculos no trajeto, realizar a manobra de desvio e retornar automaticamente para a pista.

---

## 👥 Equipe (Legião do Mal)
* Julia
* Igor Gustavo
* Gustavo
* Juan
* Vitor Emanuel

**Data de Conclusão:** 18/09/2026

---

## 🎯 Desafio e Critérios de Sucesso
O robô deveria cumprir o seguinte ciclo de funcionamento de forma autônoma:
1. Seguir a linha preta utilizando o sensor de cor.
2. Detectar um obstáculo posicionado no meio do percurso através do sensor ultrassônico.
3. Parar e desviar do objeto com uma sequência de manobras controladas por rotações dos motores.
4. Reconectar à linha preta e retomar o percurso de patrulha normalmente.

---

## ⚙️ Hardware e Componentes Utilizados
* **Bloco Programável:** LEGO MINDSTORMS EV3.
* **Atuadores:** 2x Motores EV3 nas **Portas B e C** para tração e direção diferencial.
* **Sensores:**
  * **Sensor Ultrassônico:** Utilizado para detectar obstáculos à distância.
  * **Sensor de Cor:** Utilizado para monitorar a intensidade da luz refletida e rastrear a linha preta.
* **Estrutura:** Peças e chassis do ecossistema LEGO Technic (vigas, eixos, conectores e rodas de borracha).

---

## 🧩 Lógica de Funcionamento e Programação
O programa foi estruturado em um ambiente de blocos visuais utilizando uma lógica de execução contínua (`repete para sempre`) acoplada a condicionais (`se / então`):
* **Monitoramento Simultâneo:** O robô lê continuamente a intensidade da luz refletida (para se manter na linha) e a distância frontal (para identificar barreiras).
* **Detecção de Obstáculo:** Quando o sensor ultrassônico registra uma distância crítica (menor que 12 cm no bloco / 8 cm na lógica descrita), o robô para a movimentação e emite um alerta sonoro (`"Expressions / Ouch"`).
* **Manobra de Desvio:** Executa uma sequência exata de deslocamentos direcionais baseada em rotações predefinidas (movimentação para a esquerda, avanço em linha reta, contorno à direita e realinhamento).
* **Retorno à Pista:** Utiliza o sensor de cor buscando o limiar de reflexão luminosa (intensidade `<= 15 %`) para localizar novamente a linha preta e reiniciar o ciclo de patrulha.

---

## 🚀 Abordagem STEAM Integrada
* **S (Ciências):** Aplicação de conceitos de física óptica (reflexão da luz) e propagação de ondas ultrassônicas (eco) para percepção ambiental.
* **T (Tecnologia):** Programação baseada em blocos no ecossistema EV3 para controle de portas de motores e tratamento de dados de sensores.
* **E (Engenharia):** Montagem estrutural em LEGO Technic, distribuição de peso e posicionamento geométrico estratégico dos sensores.
* **A (Artes):** Criatividade no design de montagem e implementação de feedback interativo com efeitos sonoros na detecção de barreiras.
* **M (Matemática):** Cálculos de porcentagem de intensidade luminosa (15% e 50%), limiares de distância (8cm/12cm), regulação de velocidade (30%/40%) e contagem precisa de rotações dos eixos.

---

## 📊 Evidências e Resultados
* **Status da Missão:** Cumprida com sucesso.
* **Vídeo de Demonstração:** [Acessar Vídeo no Google Drive](https://drive.google.com/file/d/1HPn_x3ivFSOkQdt-tSjgHBZJo9FBzk5D/view?usp=sharing)

---

## 💡 Aprendizados e Próximos Passos
* **Principal Aprendizado:** Compreensão prática de como integrar hardware (sensores e motores) com o fluxo lógico de programação para conferir autonomia a um sistema robótico em tempo de execução.
* **Melhorias Futuras:** Otimização da árvore de codificação para tornar a transição entre o seguimento de linha e a rotina de desvio ainda mais fluida e responsiva.
