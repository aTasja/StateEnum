# StateEnum
Класс State содержит названия состояний (enum).
Класс GameManager хранит текущее состояние в статической переменной GAME_STATE;
Класс MainMenu демострирует использование GAME_STATE;
Каждое новое состояние игры обновляет GAME_STATE. 

Далее в игре данные состояния используются например так:

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
