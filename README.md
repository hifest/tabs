# tabs

## you can write properties in any order

### properties:
| properties | method|
| ------------- |:-------------:|
| tabsContentSelector       |the class of the container in which there is a photo of a tab and the description |
| tabsParentSelector      |parent of the tab class(wrapper tabs) | 
| tabsChildSelector      |child selector of wrapper| 
| tabsActiveSelctor | actice class      |

### example: 

```javascript
        tabs({
                tabsContentSelector:'.tabcontent',
                tabsParentSelector:'.tabheader__items',
                tabsChildSelector: '.tabheader__item',
                tabsActiveSelctor:'tabheader__item_active',

        })

```

### example layout:

``` html 
<div class="preview">
        <div class="bgc_blue"></div>
        <div class="container">
            <div class="tabcontainer">
                <div class="tabcontent"> //tabsContentSelector
                    <img src="img/tabs/vegy.jpg" alt="vegy">
                    <div class="tabcontent__descr">
                        Меню "Фитнес" - это новый подход к приготовлению блюд: больше свежих овощей и фруктов. Для людей, которые интересуются спортом; активных и здоровых. Это абсолютно новый продукт с оптимальной ценой и высоким качеством!
                    </div>
                </div>
                <div class="tabcontent">//tabsContentSelector
                    <img src="img/tabs/elite.jpg" alt="elite">
                    <div class="tabcontent__descr">
                        Меню “Премиум” - мы используем не только красивый дизайн упаковки, но и качественное исполнение блюд. Красная рыба, морепродукты, фрукты - ресторанное меню без похода в ресторан!
                    </div>
                </div>
                <div class="tabcontent">//tabsContentSelector
                    <img src="img/tabs/post.jpg" alt="post">
                    <div class="tabcontent__descr">
                        Наше специальное “Постное меню” - это тщательный подбор ингредиентов: полное отсутствие продуктов животного происхождения. Полная гармония с собой и природой в каждом элементе! Все будет Ом!
                    </div>
                </div>
                <div class="tabcontent">//tabsContentSelector
                    <img src="img/tabs/vegy.jpg" alt="vegy">
                    <div class="tabcontent__descr">
                        Меню "Сбалансированное" - это соответствие вашего рациона всем научным рекомендациям. Мы тщательно просчитываем вашу потребность в к/б/ж/у и создаем лучшие блюда для вас.
                    </div>
                </div>
                <div class="tabheader">
                    <h3>Выберите стиль питания</h3>
                    <div class="tabheader__items">// tabsParentSelector
                        <div class="tabheader__item tabheader__item_active">Фитнес</div>//tabsChildSelector
                        <div class="tabheader__item">Премиум</div>//tabsChildSelector
                        <div class="tabheader__item">Постное</div>//tabsChildSelector
                        <div class="tabheader__item">Сбалансированное</div>//tabsChildSelector
                    </div>
                </div>
            </div>
            <div class="preview__life">Живи полной жизнью!</div>
        </div>
    </div>

```

### if you have a project collector then export the file like this:
 the file script.min.js and script.js spells out the exports, but import them into a file that collects the entire project:
 ```javascript
        import  tabs from './modules/tabs';  // './modules/tabs' -src in which the slider file lies
 ```
