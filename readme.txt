测试：python3 -m unittest discover -s tests/data_asset_trials -p 'test_*.py'
构建：python3 -m compileall -q fashion_data_foundry tests/data_asset_trials
验收：python3 -m fashion_data_foundry.workbench.cli fixtures/demo.json --database /tmp/fashion_data_foundry-acceptance.sqlite3
所有输入均为本地合成数据，运行不需要网络。
