Use This

```{.wavedrom}
{ "signal": [
 { "name": "CK",   "wave": "P.......",                                              "period": 2  },
 { "name": "CMD",  "wave": "x.3x=x4x=x=x=x=x", "data": "RAS NOP CAS NOP NOP NOP NOP", "phase": 0.5 },
 { "name": "ADDR", "wave": "x.=x..=x........", "data": "ROW COL",                     "phase": 0.5 },
 { "name": "DQS",  "wave": "z.......0.1010z." },
 { "name": "DQ",   "wave": "z.........5555z.", "data": "D0 D1 D2 D3" }
]}
```

```{.wavedrom}
{ "assign":[
  ["out",
    ["|",
      ["&", ["~", "a"], "b"],
      ["&", ["~", "b"], "a"]
    ]
  ]
]}
```

```{.wavedrom}
{"reg": [
  { "name": "IPO",   "bits": 8, "attr": "RO" },
  {                  "bits": 7 },
  { "name": "<o>B</o><b>R<i>K</i></b>",   "bits": 5, "attr": "RW", "type": 4 },
  { "name": "CPK",   "bits": 1 },
  { "name": "Clear", "bits": 3 },
  { "bits": 8 }
]}
```

