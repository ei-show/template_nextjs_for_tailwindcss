# 使い方

## cssファイルをmodulesとしてimportする場合

### index.js
```js
import styles from '../styles/Home.module.css'

export default function Home() {
    return (
        <button className={styles.btn}>
            commit
        </button>
    )
}
```

### Home.module.css
```css
.btn {
    @apply text-gray;
}
```

### メリット
* classNameが荒れない
* 使い回しができる
* テンプレートと相性がいい
* カスタム可能

### デメリット
* かゆいところに手が届かない
* 
* 
* 

---

## classNameに直接指定する

### index.js
```js
export default function Home() {
    return (
        <button className="bg-black text-white">
            commit
        </button>
    )
}
```

### メリット
* cssファイルどこだっけって探す必要がない
* 
* 
* 

### デメリット
* classNameが荒れる
* カスタムする場合、結局cssファイルを読み込む必要がある
* 
* 