# Статті за групами підходів (для таблиці на слайді 4)

| Група | Робота | Ідея |
|---|---|---|
| Гібридні | Kula (2015), *Metadata Embeddings for User and Item Cold-start Recommendations* (LightFM), arXiv:1507.08439 | вектор користувача й об’єкта будується з векторів їхніх метаданих |
| Глибокі з ознаками | Volkovs, Yu, Poutanen (2017), *DropoutNet*, NeurIPS | під час навчання випадково «вимикають» інформацію про взаємодії, тож модель вчиться спиратися на ознаки |
| Глибокі з ознаками | Zhu et al. (2020), *Recommendation for New Users and New Items via Randomized Training and Mixture-of-Experts Transformation* (Heater), SIGIR | випадкове навчання й суміш експертів для нових користувачів і об’єктів |
| Meta-learning | Lee et al. (2019), *MeLU*, KDD, arXiv:1908.00413 | meta-learning (на основі MAML) для швидкої адаптації до нового користувача за кількома прикладами |
| Meta-learning | Dong et al. (2020), *MAMO*, KDD | meta-learning із двома видами пам’яті (за ознаками й за задачами) |
| Meta-learning | Pan et al. (2019), *Warm Up Cold-start Advertisements* (MetaEmbedding), SIGIR | генератор початкових ID-векторів для нових оголошень на основі їхніх ознак |
| Графові | Berg, Kipf, Welling (2017), *Graph Convolutional Matrix Completion* (GCMC), arXiv:1706.02263 | графовий автокодувальник на двочастковому графі користувачі–об’єкти |
| Графові | Zhang, Chen (2020), *Inductive Matrix Completion Based on GNN* (IGMC), ICLR, arXiv:1904.12058 | індуктивна модель без ознак: працює з підграфом навколо пари користувач–об’єкт |
| Графові | Zhang et al. (2019), *STAR-GCN*, IJCAI, arXiv:1905.13129 | стекові GCN, що відновлюють вектори вузлів із замаскованими входами |
| Графові | Ying et al. (2018), *PinSage*, KDD, arXiv:1806.01973 | промислова GNN на графі в мільярди вузлів |
| Контрастні | Wei et al. (2021), *Contrastive Learning for Cold-Start Recommendation* (CLCRec), ACM Multimedia, arXiv:2107.05315 | контрастне навчання між вмістом об’єктів і колаборативним сигналом |

Перед цитуванням звірити авторів, рік і вихідні дані кожної статті.
