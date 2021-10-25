# TypingFiddle

<a href="https://typefiddle.pritudev.me">
  
![image](https://user-images.githubusercontent.com/75468116/137464679-47596cd1-041f-43eb-beca-1b566f50f64e.png)
  
</a>

<br/><br/>

<p align="center">
  
<img align="center" alt="JavaScript" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png" />
<img align="center" alt="HTML5" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/html/html.png" />
<img align="center" alt="CSS3" width="50px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" />

</p>
<br/>

## About

Typefiddle is a minimalistic typing test website with history of your test.

## Bug report or Feature request

To report anything or to request for Features you can join [discord server](https://discord.io/prituhq) and ask there.

## How to run locally

```zsh
git clone https://github.com/pritudev/typefiddle-v2.git
cd typing-test
npm install
npm start     # to start local server at `localhost:3000`
npm run build # to create production build run
```

## Contributing

## Got new theme ideas?

I'll be happy to merge your theme ideas into typing-test. To add new theme:

1. Add theme colors into `src/stylesheets/themes.scss` in following format:

```css
.theme-name {
  --bg-color: <background-color here> !important;
  --font-color: <font-color here> !important;
  --hl-color: <highlight-color here> !important;
  --fg-color: <forground-color here> !important;
}
```

> **Note:**  
> `highlight-color` is used for caret, wrong characters, timer, selected and onhover colors  
> `forground-color` is used for correctly typed characters  
> <i>Using hex codes for colors is recommended</i>

2.  Add theme name into `src/components/Header.tsx` in options:

```tsx
const options: Options = {
	time: [15, 30, 45, 60],
	theme: ["default", "mkbhd", "coral", "ocean", "azure", "forest", <theme-name>],
};
```

> **Important:**  
> theme-name in `themes.scss` and `Header.tsx` should always match otherwise themes won't work

3. Make a pull request

4. If it's good enough to merge, I'll merge it
