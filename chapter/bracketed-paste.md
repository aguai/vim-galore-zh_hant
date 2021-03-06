## 粘貼歸類 (要不爲什麼我總要設置‘粘貼’？)

粘貼歸類模式使得終端虛擬器可以區分鍵入文本和粘貼文本。

你是否曾經嘗試過向 Vim 粘貼過代碼，結果弄得一團糟？

這隻會在你通過 `cmd+v`， `shift-insert`， `middle-click` 等等命令進行粘貼時發生。
因爲那時你只是在向終端虛擬器裏丟文本。Vim 並不知道你在粘貼文本，它天真地認爲你是一個熟練的打字員。因此，它嘗試排版，但是失敗了。

如果你使用 Vim 命令集裏的粘貼，比如 `"+p` ，那這就不會成爲問題，因爲 Vim 知道你做的是粘貼操作。

爲了解決這個，你需要設置粘貼 `:set paste` ，以便獲取粘貼現狀。 參考 `:h 'paste'` 和 `:h 'pastetoggle'`.

如果你已經受夠了不停地切換 `'paste'` ，看一看這個不錯的插件能爲你做什麼：[粘貼歸類](https://github.com/ConradIrwin/vim-bracketed-paste)。

插件作者的拓展閱讀：[歡迎點擊](http://cirw.in/blog/bracketed-paste).

**Neovim**: Neovim 努力無縫地完成這些工作，並在終端虛擬器支持時自動設定粘貼歸類模式。
