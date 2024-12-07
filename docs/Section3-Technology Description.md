# Technology Description

## (中文)
Virtual Assistant 使用 Retrieval-Augmented Generation(RAG)技術進行開發。傳統的生成式語言模型通過預訓練來建立知識，但這些模型存在知識上的局限。當面對新資訊或快速變化的領域時，模型的回應可能會過時或不準確。如果要重新訓練語言模型或利用微調來增加其知識，將會耗費大量時間且需要充足的計算資源。

RAG 結合了檢索與生成兩種技術。首先，它從外部資料庫檢索與查詢相關的資料，補充語言模型的知識，使得回應更具時效性和精確性。此外，RAG 能減少對大量參數的依賴，因為檢索系統負責提供所需的資訊，生成模型則僅根據檢索結果來生成回應。這不僅能提高系統效率，還能減少模型訓練的複雜性。總的來說，RAG 在知識範圍和生成品質之間達到了平衡，尤其在需要動態更新資料的情境下，能有效提升生成式語言模型的準確性、靈活性和效率。

## (CHATGPT 翻譯)
The Virtual Assistant is developed using Retrieval-Augmented Generation (RAG) technology. Traditional generative language models build knowledge through pre-training, but these models have knowledge limitations. When faced with new information or rapidly changing fields, the model’s responses may become outdated or inaccurate. Retraining the language model or using fine-tuning to increase its knowledge can be time-consuming and require substantial computational resources.

RAG combines retrieval and generation techniques. First, it retrieves relevant information from external databases to supplement the language model’s knowledge, making the responses more timely and accurate. Additionally, RAG reduces the reliance on large parameters. Since the retrieval system provides the necessary information, the generative model only needs to generate responses based on the retrieved results. This not only improves system efficiency but also reduces the complexity of model training. Overall, RAG strikes a balance between knowledge coverage and generation quality, especially in scenarios where dynamic data updates are required, effectively improving the accuracy, flexibility, and efficiency of generative language model responses.

## 使用技術
- 開發框架: langchain 0.3
- 開發程式: python 3.12.8
- 生成式語言模型: OPENAI GPT-4（Generative Pre-trained Transformer）
- 嵌入式模型: OpenAI Embeddings
- 向量資料庫: Chroma