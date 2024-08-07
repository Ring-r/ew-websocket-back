# ew-websocket-back
experiments with websocket (back-end)

## Resources
 - [WebSockets - FastAPI](https://fastapi.tiangolo.com/advanced/websockets/).
## Environment Setup
1. **Create and activate a virtual environment:**
```shell
python3 -m venv ./.venv
source ./.venv/bin/activate
```
2. **Install the required dependencies:**
```shell
pip install -r ./requirements.in
```
## Running the Server
1. **Activate the virtual environment:**
```shell
source ./.venv/bin/activate
```
2. **Start the FastAPI server using Uvicorn:**
```shell
uvicorn main:app
```
## Client (CLI)
To interact with the WebSocket server, you can use the `wscat` command-line tool:
1. **Connect to the WebSocket server:**
```shell
wscat -c 127.0.0.1:8000/ws
```
### Test Data
When connected to the WebSocket server, you can send test data in the following JSON format:
```json
 {"action": "test-action", "data": "test-data"}
```
