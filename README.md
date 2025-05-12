@app.route('/', methods=['POST'])
def webhook():
    data = request.get_json()
    print("Received from TradingView:", data)  # <-- This shows if data arrived
    # Then send to Telegram
