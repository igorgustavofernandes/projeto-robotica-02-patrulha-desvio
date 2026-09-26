@"
# 🤖 Projeto II: Robô Patrulha com Desvio de Obstáculos (LEGO MINDSTORMS EV3)

Repositório dedicado à documentação, código e evidências do **Projeto Patrulha**, desenvolvido para a oficina de Programação e Robótica LEGO MINDSTORMS EV3 (STEAM)[cite: 1]. O objetivo principal foi projetar e programar um robô autônomo capaz de realizar um percurso utilizando o seguimento de linha, identificar obstáculos no trajeto, realizar a manobra de desvio e retornar automaticamente para a pista[cite: 1].

---

## 👥 Equipe (Legião do Mal)
* Julia[cite: 1]
* Igor Gustavo[cite: 1]
* Gustavo[cite: 1]
* Juan[cite: 1]
* Vitor Emanuel[cite: 1]

**Data de Conclusão:** 18/09/2026[cite: 1]

---

## 🎯 Desafio e Critérios de Sucesso
O robô deveria cumprir o seguinte ciclo de funcionamento de forma autônoma:
1. **Seguir a linha preta** utilizando o sensor de cor[cite: 1].
2. **Detectar um obstáculo** posicionado no meio do percurso através do sensor ultrassônico[cite: 1].
3. **Parar e desviar** do objeto com uma sequência de manobras controladas por rotações dos motores[cite: 1].
4. **Reconectar à linha preta** e retomar o percurso de patrulha normalmente[cite: 1].

---

## ⚙️ Hardware e Componentes Utilizados
* **Bloco Programável:** LEGO MINDSTORMS EV3[cite: 1].
* **Atuadores:** 2x Motores EV3 nas **Portas B e C** para tração e direção diferencial[cite: 1].
* **Sensores:**
  * **Sensor Ultrassônico:** Utilizado para detectar obstáculos à distância[cite: 1].
  * **Sensor de Cor:** Utilizado para monitorar a intensidade da luz refletida e rastrear a linha preta[cite: 1].
* **Estrutura:** Peças e chassis do ecossistema LEGO Technic (vigas, eixos, conectores e rodas de borracha)[cite: 1].

---

## 🧩 Lógica de Funcionamento e Programação
O programa foi estruturado em um ambiente de blocos visuais utilizando uma lógica de execução contínua (`repete para sempre`) acoplada a condicionais (`se / então`)[cite: 1]:
* **Monitoramento Simultâneo:** O robô lê continuamente a intensidade da luz refletida (para se manter na linha) e a distância frontal (para identificar barreiras)[cite: 1].
* **Detecção de Obstáculo:** Quando o sensor ultrassônico registra uma distância crítica (menor que 12 cm no bloco / 8 cm na lógica descrita), o robô para a movimentação e emite um alerta sonoro (`"Expressions / Ouch"`)[cite: 1].
* **Manobra de Desvio:** Executa uma sequência exata de deslocamentos direcionais baseada em rotações predefinidas (movimentação para a esquerda, avanço em linha reta, contorno à direita e realinhamento)[cite: 1].
* **Retorno à Pista:** Utiliza o sensor de cor buscando o limiar de reflexão luminosa (intensidade `<= 15 %`) para localizar novamente a linha preta e reiniciar o ciclo de patrulha[cite: 1].

---

## 🚀 Abordagem STEAM Integrada
* **S (Ciências):** Aplicação de conceitos de física óptica (reflexão da luz) e propagação de ondas ultrassônicas (eco) para percepção ambiental[cite: 1].
* **T (Tecnologia):** Programação baseada em blocos no ecossistema EV3 para controle de portas de motores e tratamento de dados de sensores[cite: 1].
* **E (Engenharia):** Montagem estrutural em LEGO Technic, distribuição de peso e posicionamento geométrico estratégico dos sensores[cite: 1].
* **A (Artes):** Criatividade no design de montagem e implementação de feedback interativo com efeitos sonoros na detecção de barreiras[cite: 1].
* **M (Matemática):** Cálculos de porcentagem de intensidade luminosa (15% e 50%), limiares de distância (8cm/12cm), regulação de velocidade (30%/40%) e contagem precisa de rotações dos eixos[cite: 1].

---

## 📊 Evidências e Resultados
* **Status da Missão:** Cumprida com sucesso[cite: 1].
* **Vídeo de Demonstração:** [Acessar Vídeo no Google Drive](https://drive.google.com/file/d/1HPn_x3ivFSOkQdt-tSjgHBZJo9FBzk5D/view?usp=sharing)[cite: 1]

---

## 💡 Aprendizados e Próximos Passos
* **Principal Aprendizado:** Compreensão prática de como integrar hardware (sensores e motores) com o fluxo lógico de programação para conferir autonomia a um sistema robótico em tempo de execução[cite: 1].
* **Melhorias Futuras:** Otimização da árvore de codificação para tornar a transição entre o seguimento de linha e a rotina de desvio ainda mais fluida e responsiva[cite: 1].
"@ | Out-File -Encoding utf8 README.md