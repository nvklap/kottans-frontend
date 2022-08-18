# kottans-frontend

[Загальна інфо про курс](https://github.com/kottans/frontend/blob/2022_UA/README.md) | [Зміст курсу](https://github.com/kottans/frontend/blob/2022_UA/contents.md) | [FAQ](https://github.com/kottans/frontend/blob/2022_UA/faq.md) | [markdown](https://help.github.com/categories/writing-on-github/)

## 0. Git Basics

0.1 [Introduction to Git and GitHub (week 1&2)](https://www.coursera.org/learn/introduction-git-github)  
Оновила знання про основні комманди та функції Git'а. Аналогія _working tree_ з _workingbench_ допомогла легше засвоїти в свою чергу, що таке **_stage area_** та **_commit_**.  
`git log --graph --oneline` можливість графічно відобразити історію бранчування та злиття гілок здалася досить цікавою.  
`git commit -a -m "comment"` буду використовувати у майбутньому для якихось маленьких правок.

<details><summary>Week 1&2</summary>

![coursera week 1](./task_git_collaboration/git-coursera-w1.PNG)

![coursera week 2](./task_git_collaboration/git-coursera-w2.PNG)

</details>

0.2 [learngitbranching.js.org](https://learngitbranching.js.org/)  
Цікаві та складні завдання. Деяка інформація зовсім заплутала, деяка навпаки домогла. Наприклад, стало легше розрізняти між собою `rebase` та `cherry-pick`. А поєднання `git fetch` та `git merge` в одній команді `git pull` здається зручним.

<details><summary>Screenshots</summary>

![learngitbranching level Introduction Sequence](./task_git_collaboration/git_01.PNG)

![learngitbranching level Push & Pull -- віддалені репозиторії в Git!](./task_git_collaboration/git_02.PNG)

</details>

0.3 pull-request до [Kottans/mock-repo](https://github.com/Kottans/mock-repo) is [successfully merged and closed](https://github.com/kottans/mock-repo/pull/999).

## 1. Linux CLI, and HTTP

1.1 [Linux Survival (4 modules)](https://linuxsurvival.com/linux-tutorial-introduction/)  
До цього знала лише декілька команд типу `cd`, `pwd`, `ls`.  
Ознайомилася з корисними командами (`mkdir`, `cp`, `cat`, `mv`, `rmdir`, `find`, `man`), які допомагають швидше справитись з певними завданнями ніж при використанні ui.  
Здвивували: команда для переміщення `mv` файлів може використовуватись також для перейменування; оператор `|`, що передає одержані дані з однієї команди - в іншу.

<details><summary>Screenshots</summary>
 
![linux quiz 1](./task_linux_cli/linux_01.PNG)

![linux quiz 2](./task_linux_cli/linux_02.PNG)

![linux quiz 3](./task_linux_cli/linux_03.PNG)

![linux quiz 4](./task_linux_cli/linux_04.PNG)

</details>

1.2 & 1.3 [HTTP: Протокол, який повинен розуміти кожний веб-розробник - Частина 1](https://code.tutsplus.com/uk/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177) & [Частина 2](https://code.tutsplus.com/uk/tutorials/http-the-protocol-every-web-developer-must-know-part-2--net-31155)  
Якийсь базовий матеріал про те як працює HTTP знала до цього. Зі статті дізналась про: існування ще й таких методів як `HEAD`, `TRACE`, `OPTIONS`; що існує і паблік кешування, яке розміщено на проксі серверах для зменшення навантаження на сервер, де розміщені потрібні дані; що актуальність кешованої версії можна контролювати за допомоги спеціальних заголовків `Cache-Control`. Крім того, цікаво, що клієнт може також брати участь у "контролі" над актуальністю контенту за допомоги заголовків у своєму запиті.

## 2. VCS (hello gitty), GitHub and Collaboration

2.1 [Introduction to Git and GitHub (week 3&4)](https://www.coursera.org/learn/introduction-git-github)

Багато цікавого і нового: воркфлоу з pr, як оновлювати свій pr; `git rebase -i` інтерактивний rebase, який має багато функцій, одна із яких дозволяє `squash` декілька комітів в один; про особливість `rebase` - переписувати історію коммітів, роблячи її лінійною, і це не завжди рекомендовано робити на колабораційних проектах; можливість на гітхабі створювати своєрідний todo list для проекта, призначати, хто за що відповідає, і за допомоги коментаря у коміті `"Close #<number-of-the issue>"` відмічати відповідний пункт закритим.

<details><summary>Week 3&4</summary>

![coursera week 3](./task_git_collaboration/git-coursera-w3.PNG)

![coursera week 4](./task_git_collaboration/git-coursera-w4.PNG)

</details>

2.2 [learngitbranching.js.org](https://learngitbranching.js.org/)

Заново пройшла ті рівні які здалися на 0 степі важкими і вони стали більш зрозумілими і легкими. Практиковалась з `rebase` і `cherry-pick`; зрозуміла що ж таке `origin` і як за допомоги команд можна пушити локальну гілку у іншу на ремоут якщо вони мають різні назви, наприклад: `git push origin foo:main`, де foo - це локальна гілка, а мейн - це віддалена.  
Здивувало, що `fetch` та `pull` можуть видаляти та створювати гілки:  
`git push origin :foo` - видалить на ремоуті гілку foo  
`git fetch origin :foo` - створить локально гілку foo

<details><summary>Screenshots</summary>

![learngitbranching level Introduction Sequence](./task_git_collaboration/git_01.PNG)

![learngitbranching level Push & Pull -- віддалені репозиторії в Git!](./task_git_collaboration/git_02.PNG)

</details>

## Intro to HTML and CSS

3.1 [Intro to HTML & CSS (week 1&2)](https://www.coursera.org/learn/html-css-javascript-for-web-developers)

<details><summary>Week 1&2</summary>

![coursera week 1](./task_html_css_intro/coursera-htmlcss01.PNG)

![coursera week 2](./task_html_css_intro/coursera-htmlcss02.PNG)

</details>

3.2 [Codecademy - Learn HTML(Eng)](https://www.codecademy.com/learn/learn-html) &  
3.3 [Codecademy - Learn CSS(Eng)](https://www.codecademy.com/learn/learn-css)

<details><summary>Screenshot</summary>

![HTML & CSS codecademy](./task_html_css_intro/codecadamy.PNG)

</details>

Загалом це було повторення та систематизація того з чим вже була знайома. Дізналась про _content model_ для HTML5, яка відносить більшість html елементів до певної [категорії](https://html.spec.whatwg.org/#content-models). Ще з цікавого та нового:

- `minlength` та `maxlength` атрібути для `<input>`;
- `&nbsp` не тільки створює проміжок між словами, але й робить їх _nonbreakable_;
- `<a>` є одночасно рядковим та блоковим елементом: він може містити в собі блокові елементи, але за замовчуванням має поведінку рядкового елемента;
- `margin` у `float` елементів не колапсуються;
- як додавати кастомні шрифти за допомогою [`@font-face`](https://css-tricks.com/snippets/css/using-font-face-in-css/).

<details><summary>WIP</summary>

## 4. Responsive Web Design

4.1 [Responsive web design basics](https://web.dev/i18n/en/responsive-web-design-basics/)  
4.2 ~~[FLEXBOX. Вчимося верстати на флексах](https://www.youtube.com/playlist?list=PLM6XATa8CAG5mPV60dMmjMRrHVW4LmV2x)~~  
4.3 ~~[Flexbox Froggy](http://flexboxfroggy.com/)~~  
4.4 [CSS Grid Layout](https://www.youtube.com/watch?v=GV92IdMGFfA&list=PLM6XATa8CAG5pXQrW_kDaeZb_uIAMNZIm)  
4.5 [Grid Garden](http://cssgridgarden.com/)

<details><summary>Flexbox Froggy</summary>

![Flexbox Froggy](./task_responsive_web_design/game_flex.PNG)

</details>

## 5. HTML & CSS Practice

[Вимоги](https://github.com/kottans/frontend/blob/2022_UA/tasks/html-css-popup.md) | [nav section rules](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav) | [checkbox video](https://www.youtube.com/watch?v=E6kLaaQFctU&ab_channel=VadimMakeev)

## 6. JavaScript Basics

6.1 [Intro to JS](https://www.coursera.org/learn/html-css-javascript-for-web-developers/home/week/4)  
6.2

- ~~[Basic JavaScript](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/)~~
- ~~[ES6 Challenges ](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/#es6) перші 17~~
- [Basic Data Structures](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/#basic-data-structures)
- [Basic Algorithm Scripting](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/#basic-algorithm-scripting)
- [Functional Programming ](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/#functional-programming)
- [Algorithm Scripting Challenges](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/#intermediate-algorithm-scripting) перші 11

<details><summary>Freecodecamp JS</summary>

![Basic JavaScript](./task_js_basics/freecodecamp_js_01.PNG)  
![ES6 Challenges](./task_js_basics/freecodecamp_js_02.PNG)

</details>

</details>
