# SSR (Server Side Rendering) 

**Server-side rendering (SSR)** is a popular technique for rendering a client-side single page application **(SPA)** on the server and then sending a fully rendered page to the client. This allows for dynamic components to be served as static HTML markup.

## Examples
*NextJS:*
```jsx
function Page({ data }) {
  // Render data...
}

// This gets called on every request
export async function getServerSideProps() {
  // Fetch data from external API
  const res = await fetch(`https://.../data`)
  const data = await res.json()

  // Pass data to the page via props
  return { props: { data } }
}

export default Page
```
*React:*
***Warning!: You must also do more configuration to make this example work like Babel, Webpack etc.***
```jsx
// ...

app.get('/', (req, res) => {
  const app = ReactDOMServer.renderToString(<App />);

  const indexFile = path.resolve('./build/index.html');
  fs.readFile(indexFile, 'utf8', (err, data) => {
    if (err) {
      console.error('Something went wrong:', err);
      return res.status(500).send('Oops, better luck next time!');
    }

    return res.send(
      data.replace('<div id="root"></div>', `<div id="root">${app}</div>`)
    );
  });
});

app.use(express.static('./build'));

app.listen(PORT, () => {
  console.log(`Server is listening on port ${PORT}`);
});
```

#NODEJS