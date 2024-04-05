# View in host
https://image-galery-rosy.vercel.app/
# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### Описание проекта
Проект "Оптимизированная галерея изображений на React" представляет собой веб-приложение, разработанное с использованием библиотеки React. Основной целью проекта является создание галереи изображений, которая эффективно использует методы оптимизации загрузки страницы и ресурсов, а также обеспечивает улучшенный пользовательский опыт.

### Основные компоненты
Gallery (Галерея)
Компонент Gallery отвечает за отображение списка изображений, полученных с внешнего API Unsplash. В этом компоненте применяется ленивая загрузка изображений с использованием IntersectionObserver для оптимизации загрузки изображений, когда они попадают в область видимости пользователя.

### LazyImage (Ленивое изображение)
Компонент LazyImage реализует ленивую загрузку изображений. Он использует IntersectionObserver для определения, когда изображение попадает в область видимости, и тогда начинает загрузку изображения. Это позволяет уменьшить начальную нагрузку на страницу и улучшить производительность.

### PerformanceInfo (Информация о производительности)
Компонент PerformanceInfo предоставляет информацию о производительности приложения. Здесь можно отобразить данные о времени загрузки отдельных ресурсов и страницы, собранные с помощью Performance Web APIs, таких как Navigation Timing и Resource Timing API.

### Методы оптимизации
Ленивая загрузка изображений: Использование IntersectionObserver для отложенной загрузки изображений только при их появлении в области видимости пользователя.

Предзагрузка критически важных изображений: Применение <link rel="preload"> для предварительной загрузки критически важных изображений, улучшающих первоначальный опыт пользователя.

Анализ производительности: Использование Performance Web APIs для сбора данных о времени загрузки ресурсов и страницы, что позволяет выявить узкие места и оптимизировать производительность.

