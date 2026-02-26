# DXF Feb 18 Branch Creation

## Task Completed

Created a new branch called `dxffeb18` that represents the state of the repository on February 18, 2022.

## Branch Details

- **Branch name**: `dxffeb18`
- **Commit**: `e03695a0872be910cf5d0ed944777f079ac8b8da`
- **Commit message**: "Merge pull request #4127 from openscad/fix-nullgl"
- **Date**: February 18, 2022, 01:19:56 +0100

## Files Changed

The branch contains exactly **17 files changed** from the merge base (commit `8d1fa8a8851a8747a3053c790f537e921ef4355c`):

1. `src/CGALHybridPolyhedron.cc`
2. `src/CGALHybridPolyhedron.h`
3. `src/MouseSelector.cc`
4. `src/NULLGL.cc`
5. `src/cgal.h`
6. `src/cgalutils-applyops-hybrid-minkowski.cc`
7. `src/cgalutils-closed.cc`
8. `src/cgalutils-convex.cc`
9. `src/cgalutils-corefine.cc`
10. `src/cgalutils-hybrid.cc`
11. `src/cgalutils-mesh.cc`
12. `src/cgalutils-orient.cc`
13. `src/cgalutils-triangulate.cc`
14. `src/cgalutils.cc`
15. `src/cgalutils.h`
16. `src/export_png.cc`
17. `src/renderer.cc`

**Total changes**: 162 insertions(+), 197 deletions(-)

## What the Branch Contains

The branch includes two sets of related work merged on February 18, 2022:

1. **Fast-CSG Refactoring** (PR #4123) - 14 files changed
   - Refactored hybrid typedefs and templates
   - Made corefine utils templates
   - More mesh helpers templated on TriangleMesh

2. **NULLGL Fix** (PR #4127) - 3 additional files changed
   - Fixed NULLGL rendering issues
   - Updated export_png and renderer

## Branch Creation Command

```bash
git checkout -b dxffeb18 e03695a0872be910cf5d0ed944777f079ac8b8da
```

## Verification

The branch has been created successfully and exists locally. To verify:
```bash
git branch -v | grep dxffeb18
# Output: dxffeb18  e03695a08 Merge pull request #4127 from openscad/fix-nullgl
```

To switch to the branch:
```bash
git checkout dxffeb18
```

To verify the 17 files changed:
```bash
git diff 8d1fa8a8851a8747a3053c790f537e921ef4355c..dxffeb18 --stat | tail -3
# Output: 17 files changed, 162 insertions(+), 197 deletions(-)
```

## Next Steps

The branch `dxffeb18` has been created locally. To make it available on the remote repository, push it with:
```bash
git push origin dxffeb18
```

Note: Due to environment constraints, the branch could not be automatically pushed and may need to be pushed manually or through a separate mechanism.
