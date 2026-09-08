Для установки **NumPy** и **Matplotlib** вы можете использовать **Conda** или **pip** (в зависимости от того, как настроено ваше окружение).

---

### Вариант 1: Через Conda (рекомендуется, если вы работаете в Miniconda)

Откройте терминал и выполните:

```bash
conda install numpy matplotlib
```

Или, если хотите сразу указать полный путь к вашему conda:

```bash
/Users/root1/miniconda3/bin/conda install numpy matplotlib -y
```

---

### Вариант 2: Через pip

```bash
pip install numpy matplotlib
```

Или через Python из Miniconda:

```bash
/Users/root1/miniconda3/bin/pip install numpy matplotlib
```

---

### Вариант 3: Установка прямо из ячейки Jupyter Notebook

Вы можете создать новую ячейку вверху вашего `.ipynb` ноутбука и запустить:

```python
%pip install numpy matplotlib
```

---

> 💡 **Совет:** Для полного курса вам также пригодятся `seaborn` и `scipy`. Их можно установить одной командой вместе:
> ```bash
> conda install numpy matplotlib seaborn scipy scikit-learn -y
> ```

Если хотите, я могу запустить команду установки прямо сейчас в вашей среде терминала — просто дайте знать!