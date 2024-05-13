---
date: 2022-01-01
cssclasses:
  - note
Статус заметки:
  - ✂️ отрефакторить
Тема:
  - "[[Obsidian|Obsidian]]"
Тип: заметка
Раздел: "[[Картотека]]"
---


`app.workspace.activeEditor.clear()`
Удаляет весь текст из активной заметки

`app.workspace.activeEditor.getSelection()`
Вырезает выделение и возвращает его значение

`app.workspace.activeEditor.getViewData()`
Возвращает весь текст в заметке

`app.workspace.activeEditor.setViewData(text)`
Заменяет весь текст в заметке указанным текстом

`app.vault.modify(file, content)`
Заменяет содержимое указанного файла указанным контентом

`await app.vault.read(file)`
Возвращает содержимое указанного файла

`app.metadataCache.getBacklinksForFile(file)`
Возвращает отбратные ссылки на файл с указанием строки.

`app.vault.getMarkdownFiles().find(f => f.basename == "test 1")`
Найти файл по имени

`app.vault.getAbstractFileByPath("test/test 1.md")`
Найти файл по пути

`app.workspace.activeEditor.editor.getLine(0)`
Найти строку в текущем файле по номеру

`app.workspace.activeEditor.editor.setLine(0, text)`
Выбирает строку по номеру и заменяет её указанным текстом

`app.workspace.activeEditor.editor.getCursor()`
Находит номер строки и символа, где находится курсор

Таким образом теоретически я могу заменить строку, где находится курсор.

`app.workspace.activeLeaf.rebuildView()`
Обновляет активную вкладку





`this.app.fileManager.processFrontMatter(file, f => f[key] = value)`

Редактирует метаданные




`app.commands.executeCommandById(id)`
Запускает команду с указанным id.

Шаблон чтобы [[./Получить список id всех команд|получить список id всех команд]].
Текущий [[./Список id всех команд|список id всех команд]] (может меняться из-за изменений в плагинах или обновлений программы).

`app.workspace.activeEditor.clear()`
Удаляет весь текст из активной заметки

`app.workspace.activeEditor.getSelection()`
Вырезает выделение и возвращает его значение

`app.workspace.activeEditor.getViewData()`
Возвращает весь текст в заметке

`app.workspace.activeEditor.setViewData(text)`
Заменяет весь текст в заметке указанным текстом

`app.workspace.activeLeaf.setPinned(true)` — Закрепить текущую вкладку

`app.workspace.createLeafBySplit(app.workspace.activeLeaf, "vertical")`
Разделить пространство



Изменить метаданные:
```js
app.fileManager.processFrontMatter(file, (frontmatter) => { 
  frontmatter["key"] = "value"
})
```



## Obsidian api - как запустить QuickAdd

1. В Квикэдд создать любое действие с названием "Название действия".
2. В шаблоне написать код:

```js
await app.plugins.plugins.quickadd.api.executeChoice('Embed to journal');

```

Если нужно передать переменные из Темплейтера в Квикэдд:

1. В настройсках действия Квикэдд указать переменную в формате `{{VALUE:переменная}}`
2. В шаблоне написать код:

```js

await app.plugins.plugins.quickadd.api.executeChoice('Embed to journal', {переменная: значение_переменной});

```

Чтобы Темплейтер запускался автоматически при создании файла в папке, можно указать шаблон в качестве "folder template" для конкретной папки (указывается в настройках Темплейтера).




## Удаление заметок с помощью скрипта

`let note = app.vault.getMarkdownFiles().find(f => f.basename == "название")`
Находит заметку по названию.

`app.vault.trash(note)`
Удаляет найденную заметку в корзину.

Или:

`app.vault.delete(note)`
Удаляет найденную заметку безвозвратно.