(cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF'
diff --git a/README.md b/README.md
--- a/README.md
+++ b/README.md
@@ -1,8 +1,6 @@
-
+
+| Страница | Ссылка | Описание |
+|----------|--------|----------|
+| 🚀 **Трекер SL по коду ТТ** | [sl.html](./sl.html) | Поиск ТТ и метрики SL |
+| 📤 **Загрузка SL CSV на GitHub** | [index.html](./index.html) | Загрузка файлов `Sl1025.csv` и `Crit1025.csv` |
+| 🧾 **SDO экспорт** | [SDO.html](./SDO.html) | Разметка задач SDO для печати/экспорта |
EOF
)
