# ML & Agents Practice

Hands-on notebooks I wrote while learning deep learning and agentic AI (IIT Delhi Advanced AI & Deep Learning
Programme and self-study). Smaller and rougher than my main projects, kept here to show the ground I've covered.
All run on Google Colab.

| Notebook | Topic | Result |
|---|---|---|
| [agents/langgraph_prompt_chaining.ipynb](agents/langgraph_prompt_chaining.ipynb) | LangGraph `StateGraph` prompt chain: description → features → marketing copy → polished final, typed state between nodes, any OpenRouter model | 4-node pipeline |
| [deep-learning/mnist_mlp_backprop.ipynb](deep-learning/mnist_mlp_backprop.ipynb) | Dense network trained with backpropagation, dropout regularisation, every line commented | **98.1%** test accuracy |
| [deep-learning/cifar10_cnn.ipynb](deep-learning/cifar10_cnn.ipynb) | 3-block CNN with batch norm, dropout, he-normal init, early stopping + LR scheduling | 76.5% val. accuracy at epoch 13 (run stopped early, still improving) |
| [time-series/lstm_stock_forecast_reliance.ipynb](time-series/lstm_stock_forecast_reliance.ipynb) | Univariate LSTM forecasting on 25 years of daily closes, 120-day window, chronological split | Test RMSE **35.9 INR** |

## Running

Open a notebook in Colab (File → Open notebook → GitHub, or upload it) and run all cells.

- **LangGraph notebook:** needs an [OpenRouter](https://openrouter.ai) API key; it is entered with `getpass` at run time and never saved.
- **Stock notebook:** download `RELIANCE.NS` daily history as CSV from Yahoo Finance and upload it to `/content/`.
- MNIST and CIFAR-10 download automatically through Keras.

Local setup: `pip install -r requirements.txt`.

*The stock notebook is a modelling exercise, not investment advice.*

## Main projects

- [visual-product-search](https://github.com/sudhanshu-1999/visual-product-search): photo → exact SKU, embeddings + vision-LLM re-ranking, MCP tool
- [salesforce-llm-document-pipeline](https://github.com/sudhanshu-1999/salesforce-llm-document-pipeline): async Salesforce → FastAPI → Docling → LLM pipeline
- [yolov8-fall-detection](https://github.com/sudhanshu-1999/yolov8-fall-detection): real-time fall detection, mAP@50 0.909

## License

MIT
