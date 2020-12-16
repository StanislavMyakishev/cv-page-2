<script>
  import Profile from "../public/favicon.png";
</script>

<style lang="scss">
  .offset-wrapper {
    margin-top: 30px;
  }

  .links-table {
    display: inline-block;
  }

  img {
    width: 100px;
    border-radius: 50px;
    margin-top: 18px;
  }

  table {
    float: right;
    margin: 0 auto;
    border-spacing: 16px;

    a {
      display: block;
      color: #1a6dbb;
      font-size: 18px;
      text-decoration: none;
      transition: all 250ms ease-out 0s;
      transform: translate3d(0px, 0px, 0px);

      &:hover {
        transform: translate3d(0px, -1px, 0px);
      }
    }
  }

  @media only screen and (max-width: 550px) {
    img {
      display: none;
    }
  }
</style>

<div class="offset-wrapper">
  <div class="links-table">
    <img src={Profile} alt="stanislav myakishev" />
    <table>
      <tbody>
        <tr>
          <td>telegram:</td>
          <td><a href="https://t.me/smyakishev"> @smyakishev </a></td>
        </tr>
        <tr>
          <td>email:</td>
          <td>
            <a href="mailto:stanislaw.myakishev@yandex.ru">
              stanislaw.myakishev@yandex.ru
            </a>
          </td>
        </tr>
        <tr>
          <td>linkedin</td>
          <td>
            <a href="https://www.linkedin.com/in/smyakishev/"> smyakishev </a>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
