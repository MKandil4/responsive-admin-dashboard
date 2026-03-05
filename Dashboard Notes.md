## STRUCTURE

## page Structure

.page
├── sidebar ثابت
└── content يتمدد

# .page

→ الصفحة كلها display Flex
→ Sidebar + Content جنب بعض

# .sidebar

→ Logo
→ Navigation Links

- width 250px
- box-shadow
- bg-white → background-color:white
- p-20 → padding:20px
- p-relative → position:relative

# .sidebar > h3

- txt-c → text-align:center ✔️
- mt-0 → reset margin-top ✔️
- margin bottom 50px ✔️
- CSS margin-bottom 50px ✔️
- p-relative → علشان ::before & ::after ✔️
- make ::before & ::after ✔️

# .sidebar > ul > li > a

- class active ✔️
- d-flex ✔️
- align-center ✔️
- fs → 14px ✔️
- color → black
- raduis → 6 ✔️
- padding → 10 ✔️
- bg F6F6F6 ✔️
- hover ✔️

# .sidebar > ul > li > a > i

- class → fa-fw => Font Awesome Fixed Width ✔️
- Font Awesome بيجبر كل أيقونة يكون لها نفس العرض.

# .sidebar > ul > li > a > span

- font size 14px ✔️
- margin left 10px ✔️

# @ Mobil

> sidebar:

- width 58px ✔️
- padding 10 ✔️

> sidebar h3:

- font size 13px
- margin bottom 15px
- before & after (hide) display none ✔️
- span (hide Span) display none ✔️
- OR => you can make in framework class hide-mobile => display: none ✔️

## Progress Sidebar Tracker

- [✔️] Watch Video
- [✔️] Write Notes
- [✔️] Build Without Video
- [✔️] UI Idea Understood
- [✔️] Responsive Check

---

## Content

1- Head
2- Heading
3-
4-
5-
6-

- full width w-full ✔️
- over flow hidden /_علشان الإسكرووول_/ ✔️

## Head Structure

.Head
├── input (class .search)
└── icon (class .notifications) + image

## .content .head

- bg-white ✔️
- p-15 ✔️
- d-flex, align items center, justify content space between => best practies make component ✔️

## .content .head .search

- p-relative علشان حنعمل شكل البحث ✔️
- ::befor

## .content .head => input

- border 1px solid #ccc
- boeder raduis 10
- margin left 5px
- padding left 30px
- width 160px
- transitions width 0.3s

## .content .head .search input:focus

- width 200px

## .content .head .search input:focus::placeholder

- opacity:0 or color: transparent

## .content .head .icons => (i + img)

- d-flex
- align-items center

## .content .head .icons.notifications

- p-relative
- ::before => make red circle

## .content .head .icons span i

- class fa-lg

## .content .head .icons img

- width 32px
- height 32px
- margin left 15px

## Content => 1- Head

- [✔️] Watch Video
- [✔️] Write Notes
- [✔️] Build Without Video
- [✔️] UI Idea Understood
- [✔️] Responsive Check

---

## Content => 2- Static Heading + Scroll Bar

.page => h1

- p-relative
- margin 20 20 40
- ::befor & ::after

.page => Scrollbar

::-webkit-scrollbar
width: 15px;

::-webkit-scrollbar-track /_back_/
background-color: white;

::-webkit-scrollbar-thumb /_Front_/
background-color: var(--blue-color);

::-webkit-scrollbar-thumb:hover
background-color: var(--blue-alt-color);

---

## Wrapper And Widgets Boxes

## Content => 3- Wrapper

## Wrapper =>

├── Box Welcome
└── Box Quick Draft
└── Box Yearly Targets
└── Box Tickets Statistics
└── Box Latest News
└── Box Latest Tasks
└── Box Top Search Items
└── Box Latest Uploads
└── Box Last Project Progress
└── Box Reminders
└── Box Latest Post
└── Box Social Media Stats
└── Box Projects

## Content => 3- Wrapper

.Wrapper =>

- display Grid
- gap 20
- margin 0 20px

# @ Mobil

> Wrapper:

- grid-template-columns: minmax(200px, 1fr);
- margin-left: 10px;
- margin-right: 10px;
- gap: 10px;
- text center in mobile /_framework_/
- display block in mobile /_framework_/ فيها مشكلة

---

## 1- Box Welcome

├── intro => d-flex, space between ✔️
div (h2 + p) ✔️

├── image => width 200px, mb -10px, hide in mobile

├── image class avatar => Rounded, width 64px + height 64px,boxshadow,ml 20px, mt -32px

└── body => three (divs > spans) => flex:1 علشان يقسم العناصر ويكون في بينهم مسافات بالتساوي

└── a link class visit => margin 15px 15px 0 auto btn-shape

# @ Mobil

- intro => padding bottom -30px
- img .avatar => margin left 0px علشان تيجي فالنص
- body
  1- d-block
  2- div not last child margin bottom 20px

---

## 2- Box Quick Draft => Easy Without Notes

---

## 3- Box Yearly Targets

.├── targets
.├── h2
.├── p
.├── 1-div .target-row .blue
.├── 2-div .target-row .orange
.├── 3-div .target-row .green

.├── div .target-row .blue
.├──├── div .icon .center-flex w-80px height-80px mr-15px
.├──├──├── i .fa-lg .c-blue

.├──├──div .details flex:1
.├──├──├──span Money fs-14, c-grey
.├──├──├──span $20.000 d-block mt-5, mb-10 fw-bold

.├──├──├──div .progress p-relative height 4px
.├──├──├──├──span style=width:80%, .bg-blue .blue
.├──├──├──├──span 80% .bg-blue

## 4- Box Tickets Statistics => Easy Without Notes

## 5- Box News

## 6- Box Latest Tasks

## 7- Box Top Search Items

## 8- Box Uploads

## 9- Box Project Progress

## 10- Box Reminders

parnt div - position relative
h2 mt-0 mb-25
ul m-0
li > span circle

> div > p
> span

## 11- Box Post

## 12- Box Social Media

box => padding-left 70px

## 13- Box Projects - table

.responsive-table => over-flow-x: auto
table =>
full-width: 100%
min-width: 1000px

image =>
width + height 32px
raduis 50%
padding 2px
background-color white
image not first child => margin left -20px
