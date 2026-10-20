#בחירת תמונה של גירסא
FROM pyton:3.12.7-slim
#יצירת תקיה בתוך הקונטינר
WORKDIR /app
#העתקת הקובץ בלבד לפני העתקת הקוד
COPY requirements.txt
#התקנת התלויות
RUN pip install --no-cache-dir -r  requirements.txt
#העתקת הבצים לקונטיינר
COPY . 
#באיזה פורט
EXPOSE 8080
#הפעלת האפליקציה
CMD ["pyton","main.py"]

