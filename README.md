# ai-ecg-signal

During this project, I focused on creating a software module to generate synthetic electrocardiograms (ECGs) with T-wave alternation using JavaFX. The goal was to simulate the ECG cycles accurately and visually demonstrate T-wave alternation effects.

Here's how I did it:

First, I familiarized myself with the theoretical principles of ECG signal modeling. An ECG consists of various waves: P, Q, R, S, and T, each representing different phases of the heart's electrical activity. My task was to replicate these waves using mathematical functions.

Development Process:

Initial Application Setup: I built a JavaFX application that allows users to input parameters through sliders and buttons to control the amplitude, peak time, and symmetry of the ECG waves. The interface updates the ECG graph in real-time as users adjust these settings.

Wave Calculation: The core of the application is the mathematical function that calculates the values of each ECG wave over time. This function considers parameters like amplitude and timing to generate realistic waveforms. I integrated these calculations into the app, ensuring the graph accurately reflects the input values.

Graph Generation: I used JavaFX's LineChart to visualize the ECG cycles. Each wave (P, Q, R, S, and T) is represented by a series of data points calculated for every time increment from 0 to 1.3 seconds. These series are then combined to form a complete ECG cycle.

Parameter Management: For the T-wave, users can set parameters through the GUI. I hardcoded the parameters for other waves as constants, following the assignment requirements. Event handlers for sliders and buttons dynamically update the graph based on user input, providing immediate feedback.

Enhancing with T-wave Alternation:

I extended the application to simulate T-wave alternation, which is a variation in the T-wave amplitude that can occur in successive heartbeats.

Generation Interface: I added a feature where users can specify the number of ECG cycles to generate and set the alternation level of the T-wave. This was done through a new window that opens on clicking the “generation” button.

Cycle Calculation: The program generates multiple ECG cycles, each shifted in time. The T-wave alternation is applied to even-numbered cycles, creating a realistic alternation effect in the waveform. This was achieved by modifying the amplitude in a recursive manner for each cycle.

Visualization: The generated cycles are displayed in a new graph. Users can update the graph by adjusting the alternation level and highlighting cycles with visible alternation through the “MULTICOLORED” button.

Outcome:

The result is a functional GUI application that not only displays synthetic ECGs but also simulates the T-wave alternation phenomenon. Users can interactively modify parameters and visualize the impact on the ECG cycles, making it a useful tool for understanding ECG signal variations.


У цьому проекті я займався створенням програмного модуля для генерації штучних електрокардіограм (ЕКГ) з альтернацією зубця Т за допомогою JavaFX. Метою було точно змоделювати цикли ЕКГ і наочно показати ефекти альтернації зубця Т.

Ось як це відбувалося:

Спершу я ознайомився з теоретичними принципами моделювання сигналу ЕКГ. ЕКГ складається з різних хвиль: P, Q, R, S і T, кожна з яких відповідає за певні фази електричної активності серця. Мені потрібно було відтворити ці хвилі за допомогою математичних функцій.

Процес розробки:

Початкова настройка додатку: Я створив JavaFX-додаток, який дозволяє користувачам вводити параметри через слайдери та кнопки для контролю амплітуди, часу піку і симетрії хвиль ЕКГ. Інтерфейс оновлює графік ЕКГ в реальному часі при зміні цих налаштувань.

Розрахунок хвиль: Основою додатку є математична функція, яка обчислює значення кожної хвилі ЕКГ протягом часу. Ця функція враховує параметри, такі як амплітуда і час, щоб створити реалістичні хвилі. Я інтегрував ці розрахунки в додаток, забезпечуючи точне відображення графіка відповідно до введених значень.

Генерація графіка: Для візуалізації циклів ЕКГ я використовував LineChart JavaFX. Кожна хвиля (P, Q, R, S і T) представлена серією точок даних, розрахованих для кожного моменту часу від 0 до 1.3 секунд. Ці серії потім об'єднуються в повний цикл ЕКГ.

Управління параметрами: Для зубця Т параметри задаються через GUI. Параметри інших хвиль я закодував як константи відповідно до вимог завдання. Обробники подій для слайдерів і кнопок динамічно оновлюють графік на основі введення користувача, надаючи миттєвий зворотний зв'язок.

Розширення з альтернацією зубця Т:

Я розширив додаток для моделювання альтернації зубця Т, що є зміною амплітуди зубця Т, яка може виникати в наступних серцевих циклах.

Інтерфейс генерації: Я додав можливість, де користувачі можуть вказати кількість циклів ЕКГ і задати рівень альтернації зубця Т. Це зроблено через нове вікно, яке відкривається при натисканні кнопки “generation”.

Розрахунок циклів: Програма генерує кілька циклів ЕКГ, кожен зі зміщенням у часі. Альтернація зубця Т застосовується до парних циклів, створюючи реалістичний ефект альтернації у формі хвилі. Це було досягнуто шляхом рекурсивної модифікації амплітуди для кожного циклу.

Візуалізація: Згенеровані цикли відображаються на новому графіку. Користувачі можуть оновлювати графік, регулюючи рівень альтернації і підсвічуючи цикли з видимою альтернацією через кнопку “MULTICOLORED”.

Результат:

Результатом є функціональний GUI-додаток, який не лише відображає штучні ЕКГ, але й моделює феномен альтернації зубця Т. Користувачі можуть інтерактивно змінювати параметри і візуалізувати вплив на цикли ЕКГ, що робить його корисним інструментом для розуміння варіацій сигналів ЕКГ.
