#### No replacements

```jsx
<Intl id="deleteAndRestart" i18n={util.i18n} />
```

#### Single string replacement

```jsx
<Intl id="leftTheGroup" i18n={util.i18n} components={['Alice']} />
```

#### Single tag replacement

```jsx
<Intl
  id="leftTheGroup"
  i18n={util.i18n}
  components={[
    <button
      key="external-2"
      style={{ backgroundColor: 'blue', color: 'white' }}
    >
      Alice
    </button>,
  ]}
/>
```

#### Multiple string replacement

```jsx
<Intl
  id="changedSinceVerified"
  i18n={util.i18n}
  components={{
    name1: 'Alice',
    name2: 'Bob',
  }}
/>
```

#### Multiple tag replacement

```jsx
<Intl
  id="changedSinceVerified"
  i18n={util.i18n}
  components={{
    name1: (
      <button
        key="external-1"
        style={{ backgroundColor: 'blue', color: 'white' }}
      >
        Alice
      </button>
    ),
    name2: (
      <button
        key="external-2"
        style={{ backgroundColor: 'black', color: 'white' }}
      >
        Bob
      </button>
    ),
  }}
/>
```
