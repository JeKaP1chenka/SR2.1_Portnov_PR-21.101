# SR2.1_Portnov_PR-21.101
Скрипт, на случай, если ваша память забилась на маке

(Можете создать bash файл для удобства использования)

rm -rf ~/Library/Caches/*
rm -rf ~/Library/42_cache
rm -rf ~/Library/Application\ Support/Slack/Service\ Worker/CacheStorage/
rm -rf ~/Library/Application\ Support/Slack/Cache/
rm -rf ~/Library/Application\ Support/Slack/Code\ Cache/
rm -rf ~/Library/Application\ Code/Cache/*
rm -rf ~/Library/Application\ Code/CachedData/*
rm -rfv ~/Library/Caches/*
rm -rfv ~/Library/Application\ Support/Slack/Cache/*
rm -rfv ~/Library/Application\ Support/Slack/Service\ Worker/CacheStorage/*
rm -rfv ~/Library/Group\ Containers/6N38VWS5BX.ru.keepcoder.Telegram/account-570841890615083515/postbox/*
rm -rfv ~/Library/Caches
rm -rfv ~/Library/Application\ Support/Code/Cache
rm -rfv ~/Library/Application\ Support/Code/CachedData
rm -rfv ~/Library/Application\ Support/Code/CachedExtension
rm -rfv ~/Library/Application\ Support/Code/CachedExtensions
rm -rfv ~/Library/Application\ Support/Code/CachedExtensionVSIXs
rm -rfv ~/Library/Application\ Support/Code/Code\ Cache
rm -rfv ~/Library/Application\ Support/Slack/Cache
rm -rfv ~/Library/Application\ Support/Slack/Code\ Cache
rm -rfv ~/Library/Application\ Support/Slack/Service\ Worker/CacheStorage
rm -rfv ~/Library/Application\ Support/Code/User/workspaceStorage

Если что-то сломается ,то я не виноват - все делаешь на свой страх и риск ;)
У меня ничего не отваливалось после этого ,но мало ли что может случиться

#define WIDTH 80 #drfine HIGHT 80 //количество живых клеток int alive_count(int gen, int n) { int count = 0; for (int i = 0; i < n; i++) for (int j = 0; j < n; j++) if (gen[i][j] == 1 count++; return count; } //количество живых соседей int alive_neighbors_count (int gen, int n, int x, int y) { int count = 0; for (int i = x - 1; i <= x + 1; i++) for (int j = y - 1; j <= y + 1; j++) if (x != i && y != j && gen[i][j]) count++; return count; } //создание нового поколения void new_gen(int gen, int new_gen) { int anc = 0; for (int i = x - 1; i <= x + 1; i++) for (int j = y - 1; j <= y + 1; j++) { anc = alive_neighbors_count(gen, I, j); if (gen[i][j] == 0) { if (anc == 3) new_gen[i][j] = 1; } else { if (anc! = 1) new_gen[i][j] = 0; } } } void copy(int from, int to) {} void field(int **gen){ //отрисовка поля for (int i =0; i< n; i++) for (int j =0; j<n; j++) If(gen[i] [j]) printf("*") ; else printf(" ") ; } void game() { //Генерируем начальное поколение: int gen[WIDTH] [HEIGHT]; make_gen0(gen) ; //этого я не написала // Отрисовываем поле field(gen) ; char code =0; scanf("%c", code) ; while(code! = EXIT) { new_gen(gen, newgen) ; Field(newgen) ; } }
