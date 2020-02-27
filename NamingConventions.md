## 命名规范(Naming Conventions)
---

### 1. 在日常开发中，会涉及到文件，变量，常量等命名，这里列出一些常见的命名样式。

- **Camel Case**: `camelCase`，简称：***CC***
- **Pascal Case**: `PascalCase`，简称：***PC***
- **Kebab Case**: `kebab-case` ，简称：***KC***
- **Snake Case**: `snake_case` ，简称：***SC***
- **All Uppercase**: `ALL_UPPERCASE` ，简称：***AU***

&nbsp;

### 2. Java开发
- 类名：**Pascal case**, 如：**HomeController**
- 变量名：**Camel case**, 如：**agentCode**
- 静态常量名：**All uppercase**, 如：**CACHE_PREFIX**
- Yaml文件配置变量名：**Kebab case**, 如：**token-refresh-time**

&nbsp;

### 3. JavaScript开发

- 项目文件夹命名使用`kebab-case`命名

- *components*文件夹下的子文件夹，也统一使用 `kebab-case` 的风格

- 基础组件 (也就是展示类的、无逻辑的或无状态的组件) 应该全部以 `Base` 前缀开头

- 在注册组件的时候，全部使用 `PascalCase` 格式

```javascript
import MyComponent from './my-component.vue'

export default {
  name: 'MyComponent',
  components:{MyComponent}
}
```

- 子组件html中传入prop的为`kebab-case`格式，子组件接收方采用 `camelCase` 格式。

```javascript
<welcome-message greeting-text="hi"/>
    
props: {
  greetingText: String
}
```

- 事件统一使用 `kebab-case` 格式，并且以动词结尾。

&nbsp;

### 4. HTML/CSS开发
TODO

---
### 5. 参考(Reference)
- [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
- [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)
- [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)
- [Google JSON Style Guide](https://google.github.io/styleguide/jsoncstyleguide.xml)
