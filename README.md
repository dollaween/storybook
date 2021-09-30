# Storybook

Пример файла index.story.tsx

```tsx
const description = (
  <Sb.TextContainer>
    <h3>Подзаголовок в тексте</h3>
    <p>Обычный текст</p>

    <ol>
      <li>Нумерованный список</li>
    </ol>

    <ul>
      <li>Ненумерованный список</li>
    </ul>

    <code>Фрагмент кода</code>
    {/* Несколько фрагментов кода (будут отделены через запятую) */}
    <Sb.CodeBlocksList blocks={tuple<ButtonSize[]>('xs', 'sm', 'md', 'lg')} />
  </Sb.TextContainer>
);
```


