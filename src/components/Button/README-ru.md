<!--GITHUB_BLOCK-->

# Button

<!--/GITHUB_BLOCK-->

```tsx
import {Button} from '@gravity-ui/uikit';
```

Компонент `Button` используется как триггер для выполнения определенного действия. Основное назначение кнопки – запуск действия. В редких случаях кнопка используется вместо ссылок для перехода на другую страницу.

## Внешний вид

По внешнему виду компонент `Button` делится на 4 типа: базовая кнопка, контурная кнопка, плоская кнопка и контрастная кнопка.
Внешний вид кнопки определяется свойством `view`.

### Базовая кнопка

`action` — наиболее заметный тип кнопки. Используется для выполнения основного действия на экране, требующего максимального внимания.
Рекомендуется использовать не более одной такой кнопки на странице.

`normal` — тип кнопки по умолчанию. Используется для вторичных действий или когда нужно сохранить важность действия, но не слишком привлекать к нему внимание.

`raised` — кнопка, располагающаяся поверх контента в виде плавающего элемента; обычно имеет фиксированное положение.

<!--LANDING_BLOCK

<ExampleBlock
    code={`
<Button view="action" size="l">Action</Button>
<Button view="normal" size="l">Normal</Button>
<Button view="raised" size="l">Raised</Button>
`}>
    <UIKit.Button view="action" size="l">Action</UIKit.Button>
    <UIKit.Button view="normal" size="l">Normal</UIKit.Button>
    <UIKit.Button view="raised" size="l">Raised</UIKit.Button>
</ExampleBlock>

LANDING_BLOCK-->

<!--GITHUB_BLOCK-->

```tsx
<Button view="action" size="l">Action</Button>
<Button view="normal" size="l">Normal</Button>
<Button view="raised" size="l">Raised</Button>
```

<!--/GITHUB_BLOCK-->

### Контурная кнопка (`outlined`)

`outlined` — используется для вторичных действий, требующих меньшего внимания. Может использоваться как с основной кнопкой, так и без нее; при этом, если есть основная кнопка, она должна быть акцентирована.

`outlined-action`: Обычно используется как ссылка на другую страницу или внешний ресурс.

Этот тип кнопки также имеет дополнительные семантические варианты: `outlined-info`, `outlined-success`, `outlined-warning` и `outlined-danger`.

<!--LANDING_BLOCK

<ExampleBlock
    code={`
<Button view="outlined" size="l">Outlined</Button>
<Button view="outlined-action" size="l">Outlined Action</Button>
<Button view="outlined-info" size="l">Outlined Info</Button>
<Button view="outlined-success" size="l">Outlined Success</Button>
<Button view="outlined-warning" size="l">Outlined Warning</Button>
<Button view="outlined-danger" size="l">Outlined Danger</Button>
<Button view="outlined-utility" size="l">Outlined Utility</Button>
`}>
    <UIKit.Button view="outlined" size="l">Outlined</UIKit.Button>
    <UIKit.Button view="outlined-action" size="l">Outlined Action</UIKit.Button>
    <UIKit.Button view="outlined-info" size="l">Outlined Info</UIKit.Button>
    <UIKit.Button view="outlined-success" size="l">Outlined Success</UIKit.Button>
    <UIKit.Button view="outlined-warning" size="l">Outlined Warning</UIKit.Button>
    <UIKit.Button view="outlined-danger" size="l">Outlined Danger</UIKit.Button>
    <UIKit.Button view="outlined-utility" size="l">Outlined Utility</UIKit.Button>
</ExampleBlock>

LANDING_BLOCK-->

<!--GITHUB_BLOCK-->

```tsx
<Button view="outlined" size="l">Outlined</Button>
<Button view="outlined-action" size="l">Outlined Action</Button>
<Button view="outlined-info" size="l">Outlined Info</Button>
<Button view="outlined-success" size="l">Outlined Success</Button>
<Button view="outlined-warning" size="l">Outlined Warning</Button>
<Button view="outlined-danger" size="l">Outlined Danger</Button>
<Button view="outlined-utility" size="l">Outlined Utility</Button>
```

<!--/GITHUB_BLOCK-->

### Плоская кнопка (`flat`)

`flat` — используется для вспомогательных действий, требующих наименьшего внимания. Такие элементы часто встречаются в списках кнопок или иконок действий (без текста) в редакторах.

`flat-secondary` — менее акцентированная версия кнопки `flat`. Часто используется в качестве вспомогательной кнопки в диалогах и модальных окнах.

`flat-action` — обычно используется как ссылка на другую страницу или внешний ресурс.

Также имеет дополнительные семантические варианты: `outlined-info`, `outlined-success`, `outlined-warning` и `outlined-danger`.

<!--LANDING_BLOCK

<ExampleBlock
    code={`
<Button view="flat" size="l">Flat</Button>
<Button view="flat-secondary" size="l">Flat Secondary</Button>
<Button view="flat-action" size="l">Flat Action</Button>
<Button view="flat-info" size="l">Flat Info</Button>
<Button view="flat-success" size="l">Flat Success</Button>
<Button view="flat-warning" size="l">Flat Warning</Button>
<Button view="flat-danger" size="l">Flat Danger</Button>
<Button view="flat-utility" size="l">Flat Utility</Button>
`}
>
    <UIKit.Button view="flat" size="l">Flat</UIKit.Button>
    <UIKit.Button view="flat-action" size="l">Flat Action</UIKit.Button>
    <UIKit.Button view="flat-info" size="l">Flat Info</UIKit.Button>
    <UIKit.Button view="flat-success" size="l">Flat Success</UIKit.Button>
    <UIKit.Button view="flat-warning" size="l">Flat Warning</UIKit.Button>
    <UIKit.Button view="flat-danger" size="l">Flat Danger</UIKit.Button>
    <UIKit.Button view="flat-utility" size="l">Flat Utility</UIKit.Button>
</ExampleBlock>

LANDING_BLOCK-->

<!--GITHUB_BLOCK-->

```tsx
<Button view="flat" size="l">Flat</Button>
<Button view="flat-secondary" size="l">Flat Secondary</Button>
<Button view="flat-action" size="l">Flat Action</Button>
<Button view="flat-info" size="l">Flat Info</Button>
<Button view="flat-success" size="l">Flat Success</Button>
<Button view="flat-warning" size="l">Flat Warning</Button>
<Button view="flat-danger" size="l">Flat Danger</Button>
<Button view="flat-utility" size="l">Flat Utility</Button>
```

<!--/GITHUB_BLOCK-->

### Контрастная кнопка (`contrast`)

Кнопки `normal-contrast`, `outline-contrast` и `flat-contrast` выделяют действия на фоне сложного фона, например, на баннере или фоне с инверсией.

<!--LANDING_BLOCK

<ExampleBlock
    background='rgb(68, 38, 204)'
    code={`
<Button view="normal-contrast" size="l">Normal Contrast</Button>
<Button view="outlined-contrast" size="l">Outlined Contrast</Button>
<Button view="flat-contrast" size="l">Flat Contrast</Button>
`}
>
    <UIKit.Button view="normal-contrast" size="l">Normal Contrast</UIKit.Button>
    <UIKit.Button view="outlined-contrast" size="l">Outlined Contrast</UIKit.Button>
    <UIKit.Button view="flat-contrast" size="l">Flat Contrast</UIKit.Button>
</ExampleBlock>

LANDING_BLOCK-->

<!--GITHUB_BLOCK-->

```tsx
<Button view="normal-contrast" size="l">Normal Contrast</Button>
<Button view="outlined-contrast" size="l">Outlined Contrast</Button>
<Button view="flat-contrast" size="l">Flat Contrast</Button>
```

<!--/GITHUB_BLOCK-->

## Иконки

Чтобы добавить иконку в `Button`, используйте компонент [`Icon`](../Icon), который представляет собой обертку для SVG-файлов.

<!--LANDING_BLOCK

<ExampleBlock
    code={`
<Button view="outlined" size="l">
    <Icon data={Gear} size={18} />
    Start
</Button>
<Button view="outlined" size="l">
    End
    <Icon data={Gear} size={18} />
</Button>
<Button view="outlined" size="l">
    <Icon data={Gear} size={18} />
    Both
    <Icon data={Gear} size={18} />
</Button>
<Button view="outlined" size="l">
    <Icon data={Gear} size={18} />
</Button>
`}
>
    <UIKit.Button view="outlined" size="l">
        <UIKit.Icon data={() => (
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 16 16"><path fill="currentColor" fillRule="evenodd" d="M7.199 2H8.8a.2.2 0 0 1 .2.2c0 1.808 1.958 2.939 3.524 2.034a.199.199 0 0 1 .271.073l.802 1.388a.199.199 0 0 1-.073.272c-1.566.904-1.566 3.164 0 4.069a.199.199 0 0 1 .073.271l-.802 1.388a.199.199 0 0 1-.271.073C10.958 10.863 9 11.993 9 13.8a.2.2 0 0 1-.199.2H7.2a.199.199 0 0 1-.2-.2c0-1.808-1.958-2.938-3.524-2.034a.199.199 0 0 1-.272-.073l-.8-1.388a.199.199 0 0 1 .072-.271c1.566-.905 1.566-3.165 0-4.07a.199.199 0 0 1-.073-.271l.801-1.388a.199.199 0 0 1 .272-.073C5.042 5.138 7 4.007 7 2.2c0-.11.089-.199.199-.199ZM5.5 2.2c0-.94.76-1.7 1.699-1.7H8.8c.94 0 1.7.76 1.7 1.7a.85.85 0 0 0 1.274.735 1.699 1.699 0 0 1 2.32.622l.802 1.388c.469.813.19 1.851-.622 2.32a.85.85 0 0 0 0 1.472 1.7 1.7 0 0 1 .622 2.32l-.802 1.388a1.699 1.699 0 0 1-2.32.622.85.85 0 0 0-1.274.735c0 .939-.76 1.7-1.699 1.7H7.2a1.7 1.7 0 0 1-1.699-1.7.85.85 0 0 0-1.274-.735 1.698 1.698 0 0 1-2.32-.622l-.802-1.388a1.699 1.699 0 0 1 .622-2.32.85.85 0 0 0 0-1.471 1.699 1.699 0 0 1-.622-2.321l.801-1.388a1.699 1.699 0 0 1 2.32-.622A.85.85 0 0 0 5.5 2.2Zm4 5.8a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0ZM11 8a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" clipRule="evenodd"></path></svg>
        )} size={18} />
        Start
    </UIKit.Button>
    <UIKit.Button view="outlined" size="l">
        End
        <UIKit.Icon data={() => (
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 16 16"><path fill="currentColor" fillRule="evenodd" d="M7.199 2H8.8a.2.2 0 0 1 .2.2c0 1.808 1.958 2.939 3.524 2.034a.199.199 0 0 1 .271.073l.802 1.388a.199.199 0 0 1-.073.272c-1.566.904-1.566 3.164 0 4.069a.199.199 0 0 1 .073.271l-.802 1.388a.199.199 0 0 1-.271.073C10.958 10.863 9 11.993 9 13.8a.2.2 0 0 1-.199.2H7.2a.199.199 0 0 1-.2-.2c0-1.808-1.958-2.938-3.524-2.034a.199.199 0 0 1-.272-.073l-.8-1.388a.199.199 0 0 1 .072-.271c1.566-.905 1.566-3.165 0-4.07a.199.199 0 0 1-.073-.271l.801-1.388a.199.199 0 0 1 .272-.073C5.042 5.138 7 4.007 7 2.2c0-.11.089-.199.199-.199ZM5.5 2.2c0-.94.76-1.7 1.699-1.7H8.8c.94 0 1.7.76 1.7 1.7a.85.85 0 0 0 1.274.735 1.699 1.699 0 0 1 2.32.622l.802 1.388c.469.813.19 1.851-.622 2.32a.85.85 0 0 0 0 1.472 1.7 1.7 0 0 1 .622 2.32l-.802 1.388a1.699 1.699 0 0 1-2.32.622.85.85 0 0 0-1.274.735c0 .939-.76 1.7-1.699 1.7H7.2a1.7 1.7 0 0 1-1.699-1.7.85.85 0 0 0-1.274-.735 1.698 1.698 0 0 1-2.32-.622l-.802-1.388a1.699 1.699 0 0 1 .622-2.32.85.85 0 0 0 0-1.471 1.699 1.699 0 0 1-.622-2.321l.801-1.388a1.699 1.699 0 0 1 2.32-.622A.85.85 0 0 0 5.5 2.2Zm4 5.8a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0ZM11 8a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" clipRule="evenodd"></path></svg>
        )} size={18} />
    </UIKit.Button>
    <UIKit.Button view="outlined" size="l">
        <UIKit.Icon data={() => (
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 16 16"><path fill="currentColor" fillRule="evenodd" d="M7.199 2H8.8a.2.2 0 0 1 .2.2c0 1.808 1.958 2.939 3.524 2.034a.199.199 0 0 1 .271.073l.802 1.388a.199.199 0 0 1-.073.272c-1.566.904-1.566 3.164 0 4.069a.199.199 0 0 1 .073.271l-.802 1.388a.199.199 0 0 1-.271.073C10.958 10.863 9 11.993 9 13.8a.2.2 0 0 1-.199.2H7.2a.199.199 0 0 1-.2-.2c0-1.808-1.958-2.938-3.524-2.034a.199.199 0 0 1-.272-.073l-.8-1.388a.199.199 0 0 1 .072-.271c1.566-.905 1.566-3.165 0-4.07a.199.199 0 0 1-.073-.271l.801-1.388a.199.199 0 0 1 .272-.073C5.042 5.138 7 4.007 7 2.2c0-.11.089-.199.199-.199ZM5.5 2.2c0-.94.76-1.7 1.699-1.7H8.8c.94 0 1.7.76 1.7 1.7a.85.85 0 0 0 1.274.735 1.699 1.699 0 0 1 2.32.622l.802 1.388c.469.813.19 1.851-.622 2.32a.85.85 0 0 0 0 1.472 1.7 1.7 0 0 1 .622 2.32l-.802 1.388a1.699 1.699 0 0 1-2.32.622.85.85 0 0 0-1.274.735c0 .939-.76 1.7-1.699 1.7H7.2a1.7 1.7 0 0 1-1.699-1.7.85.85 0 0 0-1.274-.735 1.698 1.698 0 0 1-2.32-.622l-.802-1.388a1.699 1.699 0 0 1 .622-2.32.85.85 0 0 0 0-1.471 1.699 1.699 0 0 1-.622-2.321l.801-1.388a1.699 1.699 0 0 1 2.32-.622A.85.85 0 0 0 5.5 2.2Zm4 5.8a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0ZM11 8a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" clipRule="evenodd"></path></svg>
        )} size={18} />
        Both
        <UIKit.Icon data={() => (
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 16 16"><path fill="currentColor" fillRule="evenodd" d="M7.199 2H8.8a.2.2 0 0 1 .2.2c0 1.808 1.958 2.939 3.524 2.034a.199.199 0 0 1 .271.073l.802 1.388a.199.199 0 0 1-.073.272c-1.566.904-1.566 3.164 0 4.069a.199.199 0 0 1 .073.271l-.802 1.388a.199.199 0 0 1-.271.073C10.958 10.863 9 11.993 9 13.8a.2.2 0 0 1-.199.2H7.2a.199.199 0 0 1-.2-.2c0-1.808-1.958-2.938-3.524-2.034a.199.199 0 0 1-.272-.073l-.8-1.388a.199.199 0 0 1 .072-.271c1.566-.905 1.566-3.165 0-4.07a.199.199 0 0 1-.073-.271l.801-1.388a.199.199 0 0 1 .272-.073C5.042 5.138 7 4.007 7 2.2c0-.11.089-.199.199-.199ZM5.5 2.2c0-.94.76-1.7 1.699-1.7H8.8c.94 0 1.7.76 1.7 1.7a.85.85 0 0 0 1.274.735 1.699 1.699 0 0 1 2.32.622l.802 1.388c.469.813.19 1.851-.622 2.32a.85.85 0 0 0 0 1.472 1.7 1.7 0 0 1 .622 2.32l-.802 1.388a1.699 1.699 0 0 1-2.32.622.85.85 0 0 0-1.274.735c0 .939-.76 1.7-1.699 1.7H7.2a1.7 1.7 0 0 1-1.699-1.7.85.85 0 0 0-1.274-.735 1.698 1.698 0 0 1-2.32-.622l-.802-1.388a1.699 1.699 0 0 1 .622-2.32.85.85 0 0 0 0-1.471 1.699 1.699 0 0 1-.622-2.321l.801-1.388a1.699 1.699 0 0 1 2.32-.622A.85.85 0 0 0 5.5 2.2Zm4 5.8a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0ZM11 8a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" clipRule="evenodd"></path></svg>
        )} size={18} />
    </UIKit.Button>
    <div style={{display: 'flex', gap: '16px', alignItems: 'center'}}>
        <span>No text:</span>
        <UIKit.Button view="outlined" size="l">
            <UIKit.Icon data={() => (
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 16 16"><path fill="currentColor" fillRule="evenodd" d="M7.199 2H8.8a.2.2 0 0 1 .2.2c0 1.808 1.958 2.939 3.524 2.034a.199.199 0 0 1 .271.073l.802 1.388a.199.199 0 0 1-.073.272c-1.566.904-1.566 3.164 0 4.069a.199.199 0 0 1 .073.271l-.802 1.388a.199.199 0 0 1-.271.073C10.958 10.863 9 11.993 9 13.8a.2.2 0 0 1-.199.2H7.2a.199.199 0 0 1-.2-.2c0-1.808-1.958-2.938-3.524-2.034a.199.199 0 0 1-.272-.073l-.8-1.388a.199.199 0 0 1 .072-.271c1.566-.905 1.566-3.165 0-4.07a.199.199 0 0 1-.073-.271l.801-1.388a.199.199 0 0 1 .272-.073C5.042 5.138 7 4.007 7 2.2c0-.11.089-.199.199-.199ZM5.5 2.2c0-.94.76-1.7 1.699-1.7H8.8c.94 0 1.7.76 1.7 1.7a.85.85 0 0 0 1.274.735 1.699 1.699 0 0 1 2.32.622l.802 1.388c.469.813.19 1.851-.622 2.32a.85.85 0 0 0 0 1.472 1.7 1.7 0 0 1 .622 2.32l-.802 1.388a1.699 1.699 0 0 1-2.32.622.85.85 0 0 0-1.274.735c0 .939-.76 1.7-1.699 1.7H7.2a1.7 1.7 0 0 1-1.699-1.7.85.85 0 0 0-1.274-.735 1.698 1.698 0 0 1-2.32-.622l-.802-1.388a1.699 1.699 0 0 1 .622-2.32.85.85 0 0 0 0-1.471 1.699 1.699 0 0 1-.622-2.321l.801-1.388a1.699 1.699 0 0 1 2.32-.622A.85.85 0 0 0 5.5 2.2Zm4 5.8a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0ZM11 8a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" clipRule="evenodd"></path></svg>
        )} size={18} />
        </UIKit.Button>
    </div>
</ExampleBlock>

LANDING_BLOCK-->

<!--GITHUB_BLOCK-->

```tsx
<Button view="outlined" size="l">
    <Icon data={Gear} size={18} />
    Start
</Button>
<Button view="outlined" size="l">
    End
    <Icon data={Gear} size={18} />
</Button>
<Button view="outlined" size="l">
    <Icon data={Gear} size={18} />
    Both
    <Icon data={Gear} size={18} />
</Button>
<Button view="outlined" size="l">
    No text:
    <Icon data={Gear} size={18} />
</Button>
```

<!--/GITHUB_BLOCK-->

## Состояния

`Button` может иметь разные состояния:

`disabled` — когда взаимодействие с кнопкой по каким-либо причинам недоступно.

`loading` — когда в фоновом режиме выполняются асинхронные процессы.

`selected` — когда пользователь может может включить (**Enable**) или отключить (**Disable**) кнопку.

<!--LANDING_BLOCK

<ExampleBlock
    code={`
<Button size="l" disabled>Disabled</Button>
<Button size="l" loading>Loading</Button>
<Button size="l" selected>Selected</Button>
`}
>
    <UIKit.Button size="l" disabled>Disabled</UIKit.Button>
    <UIKit.Button size="l" loading>Loading</UIKit.Button>
    <UIKit.Button size="l" selected>Selected</UIKit.Button>
</ExampleBlock>

LANDING_BLOCK-->

<!--GITHUB_BLOCK-->

```tsx
<Button size="l" disabled>Disabled</Button>
<Button size="l" loading>Loading</Button>
<Button size="l" selected>Selected</Button>
```

<!--/GITHUB_BLOCK-->

## Размер

Размер `Button` можно настроить с помощью свойства `size`. Размер по умолчанию — `m`.

<!--LANDING_BLOCK

<ExampleBlock
    code={`
<Button size="xs">XS Size</Button>
<Button size="s">S Size</Button>
<Button size="m">M Size</Button>
<Button size="l">L Size</Button>
<Button size="xl">XL Size</Button>
`}
>
    <UIKit.Button size="xs">XS Size</UIKit.Button>
    <UIKit.Button size="s">S Size</UIKit.Button>
    <UIKit.Button size="m">M Size</UIKit.Button>
    <UIKit.Button size="l">L Size</UIKit.Button>
    <UIKit.Button size="xl">XL Size</UIKit.Button>
</ExampleBlock>

LANDING_BLOCK-->

<!--GITHUB_BLOCK-->

```tsx
<Button size="xs">XS Size</Button>
<Button size="s">S Size</Button>
<Button size="m">M Size</Button>
<Button size="l">L Size</Button>
<Button size="xl">XL Size</Button>
```

<!--/GITHUB_BLOCK-->

## Ширина

Для управления поведением компонента `Button` внутри контейнера используйте свойство `width`:

`auto` — ограничивает максимальную ширину кнопки, скрывая переполняющее содержимое с помощью многоточия.

`max` — подгоняет ширину кнопки под размер родительского контейнера, также скрывая переполняющее содержимое с помощью многоточия.

<!--LANDING_BLOCK

<ExampleBlock
    code={`
<Button>Default</Button>
<Button width="auto">Auto</Button>
<Button width="max">Max</Button>
`}
>
    <div style={{width: 100, border: '2px dashed gray'}}>
        <h4 style={{textAlign: 'center'}}>Default</h4>
        <p>
            <UIKit.Button>Text</UIKit.Button>
        </p>
        <p>
            <UIKit.Button>Very Long Text</UIKit.Button>
        </p>
    </div>
    <div style={{width: 100, border: '2px dashed gray'}}>
        <h4 style={{textAlign: 'center'}}>Auto</h4>
        <p>
            <UIKit.Button width="auto">Text</UIKit.Button>
        </p>
        <p>
            <UIKit.Button width="auto">Very Long Text</UIKit.Button>
        </p>
    </div>
    <div style={{width: 100, border: '2px dashed gray'}}>
        <h4 style={{textAlign: 'center'}}>Max</h4>
        <p>
            <UIKit.Button width="max">Text</UIKit.Button>
        </p>
        <p>
            <UIKit.Button width="max">Very Long Text</UIKit.Button>
        </p>
    </div>
</ExampleBlock>

LANDING_BLOCK-->

## Форматирование краев

Свойство `pin` позволяет настраивать форму _начальных_ и _конечных_ краев элемента и обычно используется для объединения нескольких кнопок в единый блок.
Значение свойства `pin` включает названия стилей _начального_ и _конечного_ краев, разделенных дефисом, например, `round-brick`.
Доступные стили краев: `round` (по умолчанию), `circle`, `brick` и `clear`.

<!--LANDING_BLOCK

<ExampleBlock
    code={`
<div>
    <Button view="action" size="l" pin="round-clear">Create</Button>
    <Button view="action" size="l" pin="brick-round">...</Button>
</div>
<div>
    <Button view="normal" size="l" pin="circle-clear">Start</Button>
    <Button view="normal" size="l" pin="brick-brick" selected>Center</Button>
    <Button view="normal" size="l" pin="clear-circle">End</Button>
</div>
<div>
    <Button view="outlined" pin="brick-clear">1</Button>
    <Button view="outlined" pin="clear-clear">2</Button>
    <Button view="outlined" pin="clear-clear">3</Button>
    <Button view="outlined" pin="clear-brick">4</Button>
</div>
`}
>
    <div>
        <UIKit.Button view="action" size="l" pin="round-clear">Create</UIKit.Button>
        <UIKit.Button view="action" size="l" pin="brick-round">...</UIKit.Button>
    </div>
    <div>
        <UIKit.Button view="normal" size="l" pin="circle-clear">Start</UIKit.Button>
        <UIKit.Button view="normal" size="l" pin="brick-brick" selected>Center</UIKit.Button>
        <UIKit.Button view="normal" size="l" pin="clear-circle">End</UIKit.Button>
    </div>
    <div>
        <UIKit.Button view="outlined" pin="brick-clear">1</UIKit.Button>
        <UIKit.Button view="outlined" pin="clear-clear">2</UIKit.Button>
        <UIKit.Button view="outlined" pin="clear-clear">3</UIKit.Button>
        <UIKit.Button view="outlined" pin="clear-brick">4</UIKit.Button>
    </div>
</ExampleBlock>

LANDING_BLOCK-->

<!--GITHUB_BLOCK-->

```tsx
<div>
    <Button view="action" size="l" pin="round-brick">Create</Button>
    <Button view="action" size="l" pin="brick-round">...</Button>
</div>
<div>
    <Button view="normal" size="l" pin="circle-clear">Start</Button>
    <Button view="normal" size="l" pin="brick-brick" selected>Center</Button>
    <Button view="normal" size="l" pin="clear-circle">End</Button>
</div>
<div>
    <Button view="outlined" pin="brick-clear">1</Button>
    <Button view="outlined" pin="clear-clear">2</Button>
    <Button view="outlined" pin="clear-clear">3</Button>
    <Button view="outlined" pin="clear-brick">4</Button>
</div>
```

<!--/GITHUB_BLOCK-->

## Свойства

| Имя          | Описание                                                                    |               Тип               | Значение по умолчанию |
| :----------- | :-------------------------------------------------------------------------- | :-----------------------------: | :-------------------: |
| children     | Содержимое кнопки. Можно использовать как текст, так и компонент `<Icon/>`. |           `ReactNode`           |                       |
| className    | HTML-атрибут `class`.                                                       |            `string`             |                       |
| component    | Переопределяет корневой компонент.                                          |       `ElementType<any>`        |      `"button"`       |
| disabled     | Включает или отключает состояние `disabled`.                                |             `false`             |        `false`        |
| extraProps   | Дополнительные свойства.                                                    |            `Record`             |                       |
| href         | HTML-атрибут `href`.                                                        |            `string`             |                       |
| id           | HTML-атрибут `id`.                                                          |            `string`             |                       |
| loading      | Включает или отключает состояние `loading`.                                 |             `false`             |        `false`        |
| onBlur       | Обработчик события `blur`.                                                  |           `Function`            |                       |
| onClick      | Обработчик события `click`.                                                 |           `Function`            |                       |
| onFocus      | Обработчик события `focus`.                                                 |           `Function`            |                       |
| onMouseEnter | Обработчик события `mouseenter`.                                            |           `Function`            |                       |
| onMouseLeave | Обработчик события `mouseleave`.                                            |           `Function`            |                       |
| pin          | Задает стиль краев кнопки.                                                  |            `string`             |    `"round-round"`    |
| qa           | HTML-атрибут `data-qa`, используется для тестирования.                      |            `string`             |                       |
| rel          | HTML-атрибут `rel`.                                                         |            `string`             |                       |
| selected     | Включает или отключает состояние `selected`.                                |                                 |                       |
| size         | Задает размер кнопки.                                                       |            `string`             |         `"m"`         |
| style        | HTML-атрибут `style`.                                                       |      `React.CSSProperties`      |                       |
| tabIndex     | HTML-атрибут `tabIndex`.                                                    |            `number`             |                       |
| target       | HTML-атрибут `target`.                                                      |            `string`             |                       |
| title        | HTML-атрибут `title`.                                                       |            `string`             |                       |
| type         | HTML-атрибут `type`.                                                        | `"button"` `"submit"` `"reset"` |      `"button"`       |
| view         | Задает внешний вид кнопки.                                                  |            `string`             |      `"normal"`       |
| width        | `"auto"` `"max"`                                                            |        `"auto"` `"max"`         |                       |

## API CSS

| Имя                                 | Описание                               |
| :---------------------------------- | :------------------------------------- |
| `--g-button-text-color`             | Цвет текста.                           |
| `--g-button-text-color-hover`       | Цвет текста при ховере.                |
| `--g-button-background-color`       | Цвет фона.                             |
| `--g-button-background-color-hover` | Цвет фона при ховере.                  |
| `--g-button-border-width`           | Ширина границы.                        |
| `--g-button-border-color`           | Цвет границы.                          |
| `--g-button-border-style`           | Стиль границы.                         |
| `--g-button-focus-outline-width`    | Толщина контура при получении фокуса.  |
| `--g-button-focus-outline-color`    | Цвет контура при получении фокуса.     |
| `--g-button-focus-outline-style`    | Стиль контура при получении фокуса.    |
| `--g-button-focus-outline-offset`   | Смещение контура при получении фокуса. |
| `--g-button-height`                 | Высота (высота строки).                |
| `--g-button-padding`                | Боковые отступы.                       |
| `--g-button-border-radius`          | Радиус скругления углов.               |
| `--g-button-font-size`              | Размер шрифта текста.                  |
| `--g-button-icon-size`              | Размер иконки.                         |
| `--g-button-icon-offset`            | Смещение иконки.                       |