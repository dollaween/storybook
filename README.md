# Storybook

Пример использования компонентов:

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

    {/* Вариант, где таблица строится автоматически исходя из объекта */}
    <Sb.Table data={{
      lg: 'Большой размер',
      md: 'Средний размер'
    }} />

    {/* Вариант таблицы, где каждую ячейку назначаем вручную */}
    <Sb.Table>
      <Sb.Tr>
        <Sb.Td>Ячейка 1</Sb.Td>
        <Sb.Td>Ячейка 2</Sb.Td>
      </Sb.Tr>
    </Sb.Table>

    <Sb.Keyboard data={{
      enter: 'Применить',
      esc: 'Отменить'
    }} />

  </Sb.TextContainer>
);
```


