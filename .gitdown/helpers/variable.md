### Variables

<!-- gitdown: off -->
```json
{"gitdown": "variable"}
```
<!-- gitdown: on -->

Prints the value of a property defined under a parser `variable.scope` configuration property. Throws an error if property is not set.

#### Example

<!-- gitdown: off -->
```js
var gitdown;

gitdown = Gitdown(
    '{"gitdown": "variable", "name": "name.first"}' +
    '{"gitdown": "variable", "name": "name.last"}'
);

gitdown.config({
    variable: {
        scope: {
            name: {
                first: "Gajus",
                last: "Kuizinas"
            }
        }
    }
});
```
<!-- gitdown: on -->

#### JSON Configuration

| Name | Description | Default |
| --- | --- | --- |
| `name` | Name of the property defined under a parser `variable.scope` configuration property. | N/A |

#### Parser Configuration

| Name | Description | Default |
| --- | --- | --- |
| `variable.scope` | Variable scope object. | `{}` |