# IITH-assignment-2

#1.Repositoty Structure ASSIGNMENT2 │ ├── Metadata │ ├── results.json │ └── vocab.json │ ├── Plots │ ├── bestfit_loss.png │ ├── overfit_loss.png │ └── underfit_loss.png │ ├── Neural.ipynb # Main Colab notebook (complete implementation) └── README.md # Project documentation

#2. How to Run Training Step 1 — Open the notebook Neural.ipynb step2-Mount Google Drive from google.colab import drive drive.mount('/content/drive')

step 3 — Prepare Dataset Pride and Prejudice – Jane Austen (Project Gutenberg)

Step 4 — Train Models • Underfit Model train_model(model_under, train_dl, val_dl, ...)

• Overfit Model train_model(model_over, small_train_dl, val_dl, ...)

•Best-Fit Model train_model(model_best, train_dl_small, val_dl, ...)

Each model automatically saves a checkpoint to Drive: model_under.pth model_over.pth model_best.pth

#3.Run Inference def generate_text(model, start_tokens, gen_len=50): ...

#4.Visualizations plots/underfit_loss.png plots/overfit_loss.png plots/bestfit_loss.png

#5.Evaluation – Perplexity

val_ppl = exp(validation_loss)
