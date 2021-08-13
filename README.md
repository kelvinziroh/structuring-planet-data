# Structuring Planet Data

This is an **MDN Front-end web developer** exercise on *HTML Tables*.

The exercise focuses on *advanced table styling techniques* like:

## Styling columns using `<col>`

Example:

```
<colgroup>
    <col>
    <col>
    <col style="border: 2px solid black;">
</colgroup>
```

The exercise also focuses on *making tables accessible*.

## Adding caption to your tables using `<caption>`

Example:

`<caption>Data about the planets of our solar system...</caption>`

## Adding structure with `<thead>`, `<tbody>`, `<tfoot>`

- `<thead>` is used to markup table headers
- `<tbody>` is used to markup main information the table displays
- `<tfoot>` is used to markup table footer

Example:

```
<thead>
    <tr>
        <td colspan="2">&nbsp;</td>
        <th scope="col">Name</th>
        <th scope="col">Mass (10<sup>24</sup>kg)</th>
        <th scope="col">Diameter (km)</th>
        <th scope="col">Density (kg/m<sup>3</sup>)</th>
    </tr>
</thead>
<tfoot>
    // table footer info
</tfoot>
<tbody>
    // table main content
</tbody>
```

## Using scope attributes

scope attribute with *colgroup, rowgroup, row, col* values

Example:

```
<tr>
    <td colspan="2">&nbsp;</td>
    <th scope="col">Name</th>
    <th scope="col">Mass (10<sup>24</sup>kg)</th>
    <th scope="col">Diameter (km)</th>
    <th scope="col">Density (kg/m<sup>3</sup>)</th>
</tr>
<tr>
    <th colspan="2" rowspan="4" scope="rowgroup">Terrestial planets</th>
    <th scope="row">Mercury</th>
    <td>0.330</td>
    <td>4,879</td>
    <td>5427</td>
    <td>3.7</td>
</tr>
```

You can learn more on the [HTML Tables MDN article](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables).