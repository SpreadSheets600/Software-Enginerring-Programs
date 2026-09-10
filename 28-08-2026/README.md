# Experiment 4

## Demonstrate the use of Internal CSS in an HTML.

```html
<html>
    <head>
        <title>Home Page</title>

        <style>
            body {
                background-color: LightGreen;
            }

            h1 {
                background-color: DarkBrown;
                font-size: 300%;
                text-align: center;
                color: LightGreen;
            }

            h1 {
                font-size: 250%;
                background-color: DarkBrown;
                color: LightGreen;
            }

            td {
                font-size: 200%;
            }

            table {
                color: DarkBrown;
            }
        </style>
    </head>

    <body>
        <h1>Table Creation</h1>

        <table>
            <tr>
                <th>Product</th>
                <th>Category</th>
                <th>Price</th>
            </tr>

            <tr>
                <td>Laptop</td>
                <td>Electronics</td>
                <td>999</td>
            </tr>

            <tr>
                <td>Chair</td>
                <td>Furniture</td>
                <td>299</td>
            </tr>
        </table>
    </body>
</html>
```

## Demonstrate the use of Inline CSS in an HTML file.

```html
<html>
    <head>
        <title>Home Page</title>
    </head>

    <body style="background-color: LightBlue;">
        <h1
            style="background-color: DarkBlue;
           font-size: 300%;
           text-align: center;"
        >
            Table Creation
        </h1>

        <table>
            <tr style="font-size: 200%; color: DarkBlue;">
                <th>Product</th>
                <th>Category</th>
                <th>Price</th>
            </tr>

            <tr style="font-size: 150%;">
                <td>Laptop</td>
                <td>Electronics</td>
                <td>999</td>
            </tr>

            <tr style="font-size: 150%;">
                <td>Chair</td>
                <td>Furniture</td>
                <td>299</td>
            </tr>
        </table>
    </body>
</html>
```

## Demonstrate the use of External CSS in an HTML file.

`stylesheet.css`

```css
body {
    background-color: Grey;
}

h1 {
    background-color: Black;
    font-size: 300%;
    text-align: center;
    color: Grey;
}

th {
    font-size: 250%;
    background-color: Black;
    color: Grey;
}

td {
    font-size: 200%;
}

table {
    color: Black;
}
```

`ECommmerce.html`

```html
<html>
    <head>
        <title>E-Commerce</title>

        <link rel="stylesheet" type="text/css" href="Stylesheet.css" />
    </head>

    <body>

    </body>
</html>
```
