# react-multi-step-form


## Getting Started
Follow the instruction given bellow 

```shell
npm install react-multi-step-form
```

## Example
```js
import React, { useState } from 'react'
import {useMultistepForm} from 'react-multi-step-form';
impot Form1 from "./Form1
impot Form2 from "./Form2
impot Form3 from "./Form3


const MyComponent = () => {
    const {next,back,step,isLastStep,isFirstStep} = useMultistepForm([<Form1/>,<Form2/>,<Form3/>]);


const Submit = ()=>{
if(!isLastStep}{
next()
}
}

    return (  <div>
          {step}
          {!isFirstStep &&<button onClick={back}>Back <button/>}
          <button onClick={Submit}>Next <button/>
          </div>
    )
}

