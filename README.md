# StateEnum
Класс State содержит названия состояний (enum).<br />
Класс GameManager хранит текущее состояние в статической переменной GAME_STATE.<br />
Класс MainMenu демострирует использование GAME_STATE.<br />
Каждое новое состояние игры обновляет GAME_STATE. <br />

Далее в игре данные состояния используются например так:

```
void Update()
{
  if (GameManager.GAME_SATE == GameManager.eGameState.level || GameManager.GAME_SATE == GameManager.eGameState.shootOff)
    {
        if (timerRunning)
        {
            elapsedSeconds += Time.deltaTime;
        }

    }
}
```
