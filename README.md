# item-checked-custom

> Classfunc item checked custom used antd and styled component

[![NPM](https://img.shields.io/npm/v/item-checked-custom.svg)](https://www.npmjs.com/package/item-checked-custom) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)
##Demo
https://duongdam.github.io/item-checked-custom/

## Install

```bash
npm install --save item-checked-custom

yarn add item-checked-custom
```

## Usage

```jsx
import React from "react";

import { ItemCheckedCustom } from "item-checked-custom";

const App = () => {
  const [checked, setChecked] = React.useState(false);

  const onClick = () => {
    setChecked(!checked);
  };

  return (
    <div style={{
      width: "100%",
      maxWidth: "500px",
      margin: "auto",
      marginTop: "100px",
      textAlign: "center"
    }}>

      Default
      <ItemCheckedCustom
        width={"250px"}
        checked={checked}
        onClick={onClick}
        margin={"10px"}
      />

      With border radius
      <ItemCheckedCustom
        name={"ClassFunc checked"}
        border={"1px"}
        borderRadius={"10px"}
        checked={checked}
        onClick={onClick}
        margin={"10px"}
      />

      With border radius text color
      <ItemCheckedCustom
        name={"ClassFunc checked"}
        border={"1px"}
        borderRadius={"10px"}
        checked={checked}
        onClick={onClick}
        margin={"10px"}
        isTextColor={true}
      />

      With change color
      <ItemCheckedCustom
        name={"ClassFunc checked"}
        border={"1px"}
        borderRadius={"10px"}
        color={'#690003'}
        borderColor={'#690003'}
        checked={checked}
        onClick={onClick}
        margin={"10px"}
        isTextColor={true}
      />

      With left number
      <ItemCheckedCustom
        border={"1px"}
        borderRadius={"10px"}
        checked={checked}
        onClick={onClick}
        margin={"10px"}
        isLeft={true}
        leftNumber={10}
      />

      Width revert
      <ItemCheckedCustom
        border={"1px"}
        margin={"10px"}
        checked={checked}
        onClick={onClick}
        isRevert={true}
        isLeft={true}
        leftNumber={10}
      />

      Width disable
      <ItemCheckedCustom
        border={"1px"}
        margin={"10px"}
        checked={checked}
        onClick={onClick}
        isRevert={true}
        offTooltip={true}
        disabled={true}
      />

      With off tooltip & disable
      <ItemCheckedCustom
        border={"1px"}
        margin={"10px"}
        checked={checked}
        onClick={onClick}
        isRevert={true}
        offTooltip={true}
        disabled={true}
      />
    </div>
  );

};

export default App;

```

## License

MIT © [duongdam](https://github.com/duongdam)
