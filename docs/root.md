# Получение Root доступа

Для установки Moonraker, Fluidd, Mainsail и т.д, а так же для печати напрямую из Orca Slicer требуется получить Root доступ.

!!! warning 
    
    Если вас устраивает стоковый веб интерфейс и Creality Print, то крайне не рекомендуется получать Root.
    
Для получения root доступа достаточно перейти в настройки принтера и выбрать пункт "Информация об учетной записи Root"

![Шаг 1](https://github.com/siper/creality-k1-wiki/blob/gh-pages/assets/root-step-1.png)

На экране с подтверждением, ждем конца таймера, ставим галочку под пунктом "Я прочитал(а) и принял(а) риски входа в систему от имени root".

![Шаг 2](https://github.com/siper/creality-k1-wiki/blob/gh-pages/assets/root-step-2.png)

После появится логин и пароль для входа по SSH, обычно логин - `root`, пароль - `creality_2023`

![Шаг 3](https://github.com/siper/creality-k1-wiki/blob/gh-pages/assets/root-step-3.png)


Готово, после данных шагов можно подключиться к принтеру с помощью SSH или SCP клиента.