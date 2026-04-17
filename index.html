from flask import Flask, render_template
from flask_socketio import SocketIO, emit
import time
import threading

app = Flask(__name__)
app.config['SECRET_KEY'] = 'secret!'
socketio = SocketIO(app)

# Background notification sender
def send_notifications():
    count = 1
    while True:
        time.sleep(5)
        message = f"Notification {count}"
        socketio.emit('new_notification', {'msg': message})
        count += 1

@app.route('/')
def index():
    return render_template('index.html')

# Start background thread
thread = threading.Thread(target=send_notifications)
thread.daemon = True
thread.start()

if __name__ == '__main__':
    socketio.run(app, debug=True)