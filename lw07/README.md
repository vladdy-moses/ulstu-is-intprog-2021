# Лабораторная работа №7 - Создание шаблона сайта при помощи React (Material UI)

## Цель работы

Освоение библиотеки компонентов Material UI при проектировании React-приложений.

## Ход выполнения работы

1. Создать новое приложение React с шаблоном TypeScript.
2. Добавить библиотеку Material UI.
3. Изменить `App.tsx` для использования компонентов библиотеки.

## Создание нового приложения и добавление библиотеки

Для создания приложения см. лабораторную работу № 6.

Информацию о Material UI можно прочитать тут: <https://mui.com/ru/>.
Также быстрый старт описан тут: <https://mui.com/getting-started/usage/>.

Чтобы подключить библиотеку к своему приложения, необходимо ввести команду `npm install @mui/material`.
И ещё одну (догадайтесь для чего): `npm install @emotion/styled @emotion/react @mui/icons-material`.

После этого измените `App.tsx` до следующего вида:

```tsx
import React from 'react';
import './App.css';
import { Box, AppBar, IconButton, Toolbar, Typography, Button, Container, Card, CardContent } from '@mui/material';
import MenuIcon from '@mui/icons-material/Menu';

function App() {
    return (
        <Box sx={{ flexGrow: 1 }}>
            <AppBar>
                <Toolbar>
                    <IconButton
                        size="large"
                        edge="start"
                        color="inherit"
                        aria-label="menu"
                        sx={{ mr: 2 }}
                    >
                        <MenuIcon />
                    </IconButton>
                    <Typography variant="h6" component="div" sx={{ flexGrow: 1 }}>
                        News
                    </Typography>
                    <Button color="inherit">Login</Button>
                </Toolbar>
            </AppBar>
            <Container>
                <Card sx={{ minWidth: 275 }}>
                    <CardContent>
                        <Typography sx={{ fontSize: 14 }} color="text.secondary" gutterBottom>
                            Test text into the card
                        </Typography>
                        <Typography variant="h5" component="div">
                            Another text into the card
                        </Typography>
                    </CardContent>
                </Card>
            </Container>
        </Box>
    );
}

export default App;
```

Как видно, в App используется несколько компонентов из MUI: Box, AppBar, Toolbar, IconButton и т.д.
Только есть проблема: карточка заезжает за панель меню.
Это надо решить.

## Создание шаблона по вашей тематике из компонентов MUI

В данном пункте вам необходимо описать компоненты хотя бы одной страницы из Вашего макета, используя библиотеку Material UI.

Например, если Вы решите описать страницу со списком товаров, то можно использовать:

- панель меню для навигации;
- карточки или таблицы для списка;
- типографию для изменения шрифта или позицинирования текста.
