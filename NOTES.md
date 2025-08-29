# or use PowerShell: Remove-Item -Recurse -Force node_modules, package-lock.json

rm -rf node_modules package-lock.json 
npm install
#####


export const homebanner = (data) => {
  if (localStorage.getItem("gamerjiToken") === null) {
    return instance
      .post(`${url.guestUrl}${routes.bannersList}`, data)
      .then((res) => {
        return res;
      });
  } else {
    return instance.post(`${url.bannerUrl}${routes.list}`, data).then((res) => {
      return res;
    });
  }
};


