## babel-plugin-collect-react-props

a plugin help you collect react application props

## usage

1. you react application

   ```js
   function Foo() {
      return (
        <div>
          <button vant="1">1</button>
          <button vant="2">1</button>
          <button vant="3">1</button>
          <button iview="4">1</button>
        </div>
      )
    }
   ```

2. babel config

    ```js
    [
      "collect-react-props",
      {
        "collectKey": [
          "vant",
          "iview"
        ]
      }
    ]
    ```

3. then you will get

   ```js
   {
     vant: ['1', '2', '3'],
     iview: ['4']
   }
   ```
