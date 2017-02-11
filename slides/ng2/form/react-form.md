## Reactive form

    <h2>Sign up reactive form</h2>
    <form (ngSubmit)="register()" [formGroup]="loginForm">
      <div class="form-group">
        <label for="username">Nom d'utilisateur</label>
        <input type="text" class="form-control" id="username" name="username" placeholder="Nom d'utilisateur" formControlName="username">
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" class="form-control" id="password" name="password" placeholder="Mot de passe" formControlName="password">
      </div>
      <button type="submit" class="btn btn-success">Se connecter</button>
    </form>
