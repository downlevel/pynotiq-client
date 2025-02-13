# PyNotiQ Client

A simple Python library to add messages to the PyNotiQ JSON queue.

## Installation

```sh
pip install git+https://github.com/downlevel/pynotiq_client.git

## Usage

```sh
from pynotiq_client import PyNotiQ

notifier = PyNotiQ(queue_file="queue.json")

notifier.add_message({
    "id" : 1
    "message": "My coole message"
})

messages = notifier.get_messages()
print(messages)
