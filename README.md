# react轻量开发

## 特点
- [react18](https://reactjs.org/),[vite](https://vitejs.dev/),[pnpm](https://pnpm.js.org/)


### action
通过判断git status来决定是否要提交
 if [[ -n "$(git status --porcelain)" ]]; then
            git add .
            git commit -m "Deploy website"
            git push origin HEAD:${{ github.event.repository.default_branch }}
          else
            echo "No changes to deploy."
          fi