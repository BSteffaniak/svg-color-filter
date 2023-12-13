`npm install --global tsx`

`tsx src/index.ts '#001122'`

Output (formatted):

> ```
> {
>     "values": [6.11039104328856, 43.21792655711988, 2322.0984829555778, 51.14937041469709, 93.94907807456532, 103.47345925178483],
>     "loss": 0.6965276572567873,
>     "filter": "filter: invert(6%) sepia(43%) saturate(2322%) hue-rotate(184deg) brightness(94%) contrast(103%);"
> }
> ```

`tsx src/index.ts '#001122' | jq .filter --raw-output`

Output:

> `filter: invert(6%) sepia(18%) saturate(6063%) hue-rotate(188deg) brightness(89%) contrast(102%);`
