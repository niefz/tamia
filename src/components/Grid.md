This component is available as a separate package: [stack-styled](https://github.com/sapegin/stack-styled). See [stack-styled docs](https://sapegin.github.io/stack-styled/) for more examples.

Equal width columns:

```jsx
<Grid numColumns={3}>
  <div>eins</div>
  <div>zwei</div>
  <div>polizei</div>
</Grid>
```

Equal width columns (responsive):

```jsx
<Grid minColumnWidth="xxxl">
  <div>foo</div>
  <div>bar</div>
</Grid>
```

Full width on small screens, horizontally stacked on larger screens:

```jsx
<Grid
  gridGap="m"
  justifyContent={[null, 'start']}
  gridAutoFlow={[null, 'column']}
>
  <span>foo</span>
  <span>bar</span>
  <span>baz</span>
</Grid>
```

Responsive footer:

```jsx
<Grid
  as="footer"
  justifyContent={[null, 'space-between']}
  justifyItems={['center', null]}
  gridAutoFlow={[null, 'column']}
>
  <div>© Chuck Norris, 1940</div>
  <div>Have a nice day!</div>
</Grid>
```
