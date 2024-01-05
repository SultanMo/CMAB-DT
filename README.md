How to run: 

```bash
pip3 install -r requirements.txt
python3 ./pucb/model/dm.py mean  # or switch `mean` to `kl`
# you could configure the number of simulations and which environments to use in dm.py
# under the `if __name__ == '__main__':` block
```
`pucb` includes the original code implementation provided by Xinyu Zhang.

The `make_distance_based_model` in `dm.py` contains the implementation of UCB-DT algorithm.

The notebook `LinUCB_DT.ipynb` comprises the implementation of LinUCB (Linear UCB), LinUCB-then-Commit, and LinUCB Distance Tuned algorithm. These implementations are evaluated on both logged (`dataset.txt`) and synthetic data.