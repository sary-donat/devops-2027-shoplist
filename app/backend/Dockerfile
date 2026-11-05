# תמונת בסיס של Python בגרסה קבועה
FROM python:3.11-slim
# תיקיית העבודה בתוך הקונטיינר
WORKDIR /app
# קודם רק קובץ התלויות, בשביל ה-cache
COPY requirements.txt .
# התקנת התלויות
RUN pip install --no-cache-dir -r requirements.txt
# אחר כך הקוד
COPY app.py .
# הפורט שהאפליקציה מאזינה לו
EXPOSE 5000
# הפעלת האפליקציה
CMD ["python", "app.py"]
