
name: Marvel-izing my repo
on: [pull_request]
jobs:
  giphy-generator:
    name: GIPHY Generator
    runs-on: ubuntu-latest
    steps:
      - name: GIPHY Generator
        id: giphy_generator
        uses: iamhughes/giphy-generator@v1
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # This token is provided by Actions, you do not need to create your own token
          GIPHY_TOKEN: ${{ secrets.GIPHY_TOKEN }} # This token should be created on giphy.com: https://developers.giphy.com/dashboard/?create=true
        with:
          rating: 'g'
          lang: 'en'
  update-readme:
    name: Update Quote README
    runs-on: ubuntu-latest
    steps:
      - uses: siddharth2016/quote-readme@main
        with:
          GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
