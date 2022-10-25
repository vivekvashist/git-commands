# git-commands

```python
'''git cat-file --batch-check --batch-all-objects #to see all objects in a repository'''
❯❯❯ git cat-file --batch-check --batch-all-objects                                                                      
0155eb4229851634a0f03eb265b69f5a2d56f341 tree 71
17c2335e639fcf15aee8c141c7b2793f261ccc45 tag 141
1f7a7a472abf3dd9643fd615f6da379c4acb3e3a blob 10
3c4e9cd789d88d8d89c1073707c3585e41b0e614 tree 101
83baae61804e65cc73a7201a7252750c76066a30 blob 10
a13e14f325fd4c808f1395f7381ad7d97eae3b27 commit 187
af01e7a3a044f0c663e3dc39b37e741c8c4eba68 commit 236
b3adeeaba2ab4626446c8f0595831e571d0f2d3d commit 235
bd9dbf5aae1a3862dd1526723246b20206e5fc37 blob 16
d670460b4b4aece5915caf5c68d12f560a9fe3e4 blob 13
d8329fc1cc938780ffdd9f94e0d364e0ea74f579 tree 36
fa49b077972391ad58037050f2a75f74e3671e92 blob 9
```

```python
''' check what's is being packed inside index file'''
❯❯❯ git verify-pack -v .git/objects/pack/pack-358d4e28d0428cecd9f8f1892cda177252630826.idx
89b36703dd37f9fc6f5d85876fc160feeb9145aa commit 243 156 12
bd9d9e03e6c0fb886aac3f91dcd55ae954a011dc commit 237 153 168
b3adeeaba2ab4626446c8f0595831e571d0f2d3d commit 235 152 321
af01e7a3a044f0c663e3dc39b37e741c8c4eba68 commit 236 153 473
17c2335e639fcf15aee8c141c7b2793f261ccc45 tag    141 127 626
a13e14f325fd4c808f1395f7381ad7d97eae3b27 commit 187 122 753
5ff124db96a64e45e4fbe5d9cb94f68fbfcff6aa tree   136 136 875
d8329fc1cc938780ffdd9f94e0d364e0ea74f579 tree   36 46 1011
deef2e1b793907545e50a2ea2ddb5ba6c58c4506 tree   136 136 1057
3c4e9cd789d88d8d89c1073707c3585e41b0e614 tree   8 19 1193 1 deef2e1b793907545e50a2ea2ddb5ba6c58c4506
0155eb4229851634a0f03eb265b69f5a2d56f341 tree   71 76 1212
83baae61804e65cc73a7201a7252750c76066a30 blob   10 19 1288
fa49b077972391ad58037050f2a75f74e3671e92 blob   9 18 1307
dc49f752f3c9608bc50fbc82d8b63bfcdd8d2ea2 blob   22055 5799 1325
033b4468fa6b2a9547a70d88d1bbe8bf3f9ed0d5 blob   9 20 7124 1 dc49f752f3c9608bc50fbc82d8b63bfcdd8d2ea2
1f7a7a472abf3dd9643fd615f6da379c4acb3e3a blob   10 19 7144
non delta: 14 objects
chain length = 1: 2 objects
.git/objects/pack/pack-358d4e28d0428cecd9f8f1892cda177252630826.pack: ok
```
