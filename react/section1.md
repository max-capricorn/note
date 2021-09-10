```tsx
import {MouseEvent, ReactChildren, ReactChild, ReactNode} from 'react'

export declare interface AppProps {
  onClick(event: MouseEvent<HTMLButtonElement>): void;
  
  children1:JSX.Element;
  // 不接受字符串
  children2: JSX.Element | JSX.Element[];
  
  children3: ReactChildren;
  
  children4: ReactChild[];
  
  children: ReactNode;
  
  functionChildren: (name: string) => ReactNode;
  // css in js
  style?: React.CSSProperties;
  // react 表单事件
  onChange: React.FormEventHandler<HTMLInputElement>;
  // 传递props 明确不转发类型的ref
  props: React.ComponentPropsWithoutRef<"button">
  
}



type Props = {
  children: React.ReactNode;
}

function Com（{childrem}: Props）{
 	return (<div>{children}</div>) 
}
```



```tsx
import React from 'react';

type AppRrops = {
  message: string
}


```

