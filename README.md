# FarmTech Solutions - Visão Computacional para Monitoramento 🌾👁️

Este repositório contém o projeto de Visão Computacional desenvolvido para a **Fase 6**, focado na implementação e comparação de modelos de detecção e classificação de objetos para a carteira de clientes da FarmTech Solutions.

## 👥 Integrantes do Grupo
* **Nome:** Matheus de S. Santos - RM: 566901
* **Nome:** Ricardo José Amorin] - RM: 567312
* **Nome:** Victor Oliveira Fedeli Tate- RM: 566823
*  **Nome:** Paulo Roberto Silva Amaral Ribeiro Junior - RM: 568413
*  **Nome:** Klaus Lohany Barbosa de Oliveira - RM: 

---

## 📂 Visão Geral do Projeto

O objetivo deste projeto é demonstrar a aplicação prática da biblioteca **YOLO (You Only Look Once)** e Redes Neurais Convolucionais (**CNN**) para identificar dois objetos específicos em cenários distintos, garantindo acurácia e performance para segurança , foi considerado um sistema de segurança de um galinheiro onde é possivel identificar galinhas ou predadores , que no caso é representado por uma raposa.

### Objetos Escolhidos:
1.  **Objeto A:** Galinha
2.  **Objeto B:** Raposa

---

## 🚀 Como Executar a Solução

Toda a lógica de treinamento e teste foi centralizada no Google Colab para facilitar a execução e o uso de GPU.

1.  **Notebook Principal:** 
2.  **Dataset:** As imagens foram rotuladas via **Make Sense IA** e organizadas no Google Drive.
3.  **Configuração:** O código realiza a conexão automática com o Drive para carregar os datasets de Treino, Validação e Teste.

---

## 📊 Metas Atingidas

### Entrega 1: Customização YOLO
- [x] Dataset de 80 imagens (40 de cada objeto).
- [x] Divisão 64/8/8 (Treino/Validação/Teste).
- [x] Rotulação completa no formato YOLO.
- [x] Simulação comparativa entre 30 e 60 épocas.
- [x] Demonstração de resultados através de prints de detecção.

### Entrega 2: Comparação de Modelos
- [x] Implementação do YOLO Adaptável (Customizado).
- [x] Implementação do YOLO Tradicional (Pré-treinado).
- [x] Treinamento de uma CNN do zero para classificação.
- [x] Análise crítica de performance, tempo de inferência e precisão.

---

## 📺 Demonstração em Vídeo


👉 **[ASSISTIR VÍDEO NO YOUTUBE] https://www.youtube.com/watch?v=YIFoNXpvJJU**


---

## 🛠️ Tecnologias Utilizadas
* **Python 3.x**
* **YOLOv5** 
* **TensorFlow/Keras** 
* **Google Colab** 
* **Make Sense IA** 

---

## 📝 Conclusões
Apesar do yolo ser uma boa ferramenta seu custo computacional eventualmente não justifica sua utilização , quando usamos o yolo padrão observamos que ele não funciona para qualquer tipo de identificação , no caso do exemplo ele não reconhece um animal em expecifico como a raposa classificando como um gato ou ovelha. Já quando usamo o yolo adaptando com o treinamento expecifico usando nosso dataset , podemos observar que ele tem um bom comportamento obtendo numero satisfatorios para uma demosntração e com portencial de ajustes para melhor resultados.
Quando treinamos uma CNN do zero utilizando a biblioteca TensorFlow obtivemos um resultado melhor com 30 epocas em relação ao resultado do yolo adaptado , e em menos tempo , enquanto o yolo demorou 36 minutos para treinar as 30 epocas com o TensorFlow demorou aproximadamente 17 minutos , um ganho de 50% no tempo de treinamento para um resultado ligeiramente melhor e com menos custo computacional.
