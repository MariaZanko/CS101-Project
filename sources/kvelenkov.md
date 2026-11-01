# Джерела та література для розбору GNN алгоритмів та Cold Start

Для аналізу алгоритмів GNN (**GraphSAGE**, **GAT**, **LightGCN**) та проблеми **Cold Start** використовуються такі фундаментальні академичні роботи та оригінальні дослідження:

---

## 1. Первоисточники алгоритмів (Original Papers)

### **GraphSAGE**
* **Назва:** *Inductive Representation Learning on Large Graphs*
* **Автори:** William L. Hamilton, Rex Ying, Jure Leskovec (Stanford University)
* **Публікація:** NIPS 2017 (NeurIPS)
* **Де знайти:** arXiv або ACM Digital Library за назвою.
* **Про що:** Введення концепції семплювання та агрегації сусідів (Sample & Aggregate), навчання функцій-агрегаторів замість фіксованих ембеддингів, забезпечення індуктивного навчання (Inductive Learning) для невідомих вузлів через їх атрибути (Node Features).
* **Як використано:** Для опису принципу індуктивного навчання, масштабованості та поведінки під час появі нових вузлів.

### **GAT (Graph Attention Networks)**
* **Назва:** *Graph Attention Networks*
* **Автори:** Petar Veličković, Guillem Cucurull, Arantxa Casanova, Adriana Romero, Pietro Liò, Yoshua Bengio
* **Публікація:** ICLR 2018
* **Де знайти:** OpenReview або arXiv за назвою.
* **Про що:** Використання механізму Self-Attention для розрахунку вагових коефіцієнтів зв'язків між вузлами в графі. Висвітлення обчислювальної складності $\mathcal{O}(\vert{}V\vert{} + \vert{}E\vert{})$.
* **Як використано:** Для пояснення адаптивного зважування сусідів, високої точності моделі та її вимог до наявності сусідніх вузлів у графі.

### **LightGCN**
* **Назва:** *LightGCN: Simplifying and Powering Graph Convolution Network for Recommendation*
* **Автори:** Xiangnan He, Kuan Deng, Xiang Wang, Yan Li, Yongdong Zhang, Meng Wang
* **Публікація:** ACM SIGIR 2020
* **Де знайти:** ACM Digital Library або arXiv за назвою.
* **Про що:** Спрощення класичного GCN для задач рекомендацій — вилучення нелінійних активацій та вагових матриць $W$. Лінійна пропагація ембеддингів за графом взаємодій (User-Item Interaction Graph).
* **Як використано:** Для опису алгоритму коллаборативної фільтрації, його швидкодії та повної залежності від топології (ID вузлів).

---

## 2. Джерела з проблематики Cold Start у рекомендаціях

### **Schein et al. (2002)**
* **Назва:** *Methods and Metrics for Cold-Start Recommendations*
* **Автори:** Andrew I. Schein, Alexandrin Popescul, Lyle H. Ungar, David M. Pennock
* **Публікація:** ACM SIGIR 2002
* **Де знайти:** ACM Digital Library за назвою.
* **Про що:** Фундаментальна робота, що формулює проблему «холодного старту» як окрему задачу через неможливість застосування класичної колаборативної фільтрації за відсутності ребер/історії.
* **Як використано:** Постановка проблеми для Слайду 12 та обґрунтування того, чому топологічні моделі (як LightGCN) провалюються без наявності зв'язків у графі.