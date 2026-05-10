**PERTAMA KALI (hanya dilakukan sekali)**

```bash
# 1. Install python
sudo apt update && sudo apt upgrade -y

# 2. Install python3-venv
sudo apt install python3.12-venv

# 3. Masuk ke folder project
cd path/folder/project/kamu

# 4. Buat virtual environment
python3 -m venv venv

# 5. Aktifkan
source venv/bin/activate

# 6. Install semua library
pip install pandas numpy matplotlib seaborn scikit-learn ipykernel

# 7. Install semua library
pip install pandas numpy matplotlib seaborn scikit-learn ipykernel

# 8. Install xgboost
pip install xgboost

# 9. Daftarkan ke VS Code
python -m ipykernel install --user --name=venv --display-name "Python (venv)"
```

Lalu di VS Code klik **"Select Kernel"** (pojok kanan atas notebook) → pilih **"Python (venv)"**

---

**SETIAP KALI MAU KERJA**

```bash
# 1. Masuk ke folder project
cd path/folder/project/kamu

# 2. Aktifkan
source venv/bin/activate

# 3. Buka VS Code
code .
```

---

**SETELAH SELESAI KERJA**

```bash
deactivate
```

---

**Tanda-tanda berhasil:**
- Saat venv aktif → ada tulisan `(venv)` di depan terminal
- Saat venv mati → tulisan `(venv)` hilang
- Notebook bisa jalan → tidak ada error `ModuleNotFoundError`
