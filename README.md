# embed-base-model

## version
    version 0.1.1

## Installation
    pip install embed-base-model

## How to
    from embedmodel improt EmbedModelBase

    class Test(EmbedModelBase):

        def _load_model(self, model_path):
            return AutoModel.from_pretrained(model_path).to(device=self.device)

        def _load_tokenizer(self, model_path):
            return AutoTokenizer.from_pretrained(model_path)
            