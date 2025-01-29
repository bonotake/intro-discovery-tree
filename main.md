---
marp: true
theme: default
style: |
  .columns {
    display: grid;
    gap: 1rem;
  }
  .columns-1-1 {
    grid-template-columns: 1fr 1fr;
  }
  .columns-2-1 {
    grid-template-columns: 2fr 1fr;
  }
  .columns-1-2 {
    grid-template-columns: 1fr 2fr;
  }
  .columns-3-1 {
    grid-template-columns: 3fr 1fr;
  } 
  .columns-3-2 {
    grid-template-columns: 3fr 2fr;
  }
  .columns-2-3 {
    grid-template-columns: 2fr 3fr;
  }
  .paper-reference {
    font-size: 0.8em;
    position: absolute; 
    bottom: 1em; 
    left: 4em; 
    right: 3em;
  }
  .dialogue-line1 {
    position: absolute;
    top: 4.8em;
    left: 10em;
    width: 20em;
    height: 6em;
    font-size: 1.2em;
    font-weight: bold;
    display: flex;
    align-items: center;
    justify-content: center;
    word-wrap: break-word;
    overflow-wrap: break-word;
  }

  .dialogue-line2 {
    position: absolute;
    top: 11.5em;
    left: 3em;
    width: 20em;
    height: 6em;
    font-size: 1.2em;
    font-weight: bold;
    display: flex;
    align-items: center;
    justify-content: center;
    word-wrap: break-word;
    overflow-wrap: break-word;
  }

  .dialogue-incongruent {
    position: absolute;
    bottom: 10px;
    right: 100px;
    font-size: 1.8em;
    font-weight: bold;
    display: flex;
    align-items: center;
    justify-content: right;
    color: #c00000;
  }

  .dialogue-congruent {
    position: absolute;
    bottom: 10px;
    right: 100px;
    font-size: 1.8em;
    font-weight: bold;
    display: flex;
    align-items: center;
    justify-content: right;
    color: #00a000;
  }

  .dialogue-page {
    height: 100vh;
    display: flex;
    flex-direction: column;
  }

  .model-diagram {
    text-align: center;
    position: absolute;
    top: 65%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
  }

---
# ディスカバリーツリーについて

ぼのたけ 今井健男

---
# ディスカバリーツリーとは

やるべき活動アイテムとその進捗をツリーで示したもの。

FASTではプロダクトバックログの代わりに利用するのが推奨されている。

<div style="text-align: center;">

![h:350](images/tree0.png)

</div>

---
# 作り方・使い方（1）

<div class="columns columns-1-1">

<div>

1. 目的・アウトカムを木のルートにする
2. 着手するアイテムを解くべき課題と見立て、その課題を解消するためのアイテムを下に並べる。これにより、

     - 上にあるアイテムは、そのアイテムのwhyを示し、
     - 下にあるアイテムは、そのアイテムのhowを示すようになる。

</div>

<div>

<div style="text-align: center; position: relative; top: -150px;">

![h:680](images/tree-items.png)


</div>

</div>

---

# 作り方・使い方（2）

<div class="columns columns-3-2">

<div style="font-size: 0.9em;">

基本的には、着手するアイテムを解くべき課題と見立て、その課題を解消するためのアイテムを下に並べていくようにする。

- 子アイテムが全て解消されれば、対象アイテムの課題も解消されるようにする
  - 後で足りないものが出てくれば適時追加すれば良い
- 子アイテムとしては、主に以下の2つ
  - 対象アイテムの課題を分割した部分課題
  - アイテムの課題を解消するためのアイテム（ソリューション）

</div>


<div style="text-align: center; position: relative; top: -150px;">

![h:680](images/tree-items.png)


</div>

</div>

---

# 例1: 「ユーザー登録機能の改善」ディスカバリー

<div style="text-align: center;">

![h:500](images/tree1_discovery.png)

</div>

---

# 例2: 「商品検索フィルターの改善」デザイン

<div style="text-align: center;">

![h:500](images/tree2_design.png)

</div>

---

# 例3: 「注文キャンセル機能」デリバリー

<div style="text-align: center;">

![h:500](images/tree3_delivery.png)

</div>

---

# 進捗の表現（オンライン版）

<div style="font-size: 0.8em; text-align: center;">

miroやMuralを利用する場合、付箋を色分けして進捗を表す。
（この例では、黄色：ToDo, オレンジ：WIP, 青：Done）
子が WIP の場合、親も WIP になる

</div>

<div style="text-align: center;">

![h:350](images/tree0.png)

</div>


---

<div style="position: absolute; top: 500px; background-color: #f0f0f0;">

# <span style="color:rgb(0, 139, 160);">　進捗の表現（オフライン版）　</span>

</div>

![bg](images/physical.png)

<div class="paper-reference">

YouTube ["Quick Discovery Tree Overview"](https://youtu.be/niIW3FsClVY?si=sfzVVnktrt5-25HB) より

</div>


---

# 進捗の表現（オフライン版）

![bg opacity:0.4](images/physical.png)

<div style="font-size: 1.2em; text-align: center;">

WIPは角にカギカッコを書き、Doneは対角線に斜線を引く

</div>

<div class="columns columns-1-1">

<div style="text-align: center;">

![w:450](images/wip.png)

</div>

<div style="text-align: center;">

![w:450](images/done.png)

</div>

</div>

