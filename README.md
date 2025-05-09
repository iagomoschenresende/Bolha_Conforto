### Iniciar o ambiente virtual -> venv\Scripts\activate

### Imports necessários:
from datetime import datetime, timezone
from flask import Flask, render_template, url_for, request, redirect, flash
from flask_sqlalchemy import SQLAlchemy
from werkzeug.security import generate_password_hash, check_password_hash
from flask_login import UserMixin, LoginManager, login_user, login_required, logout_user, current_user
from flask_migrate import Migrate
from sqlalchemy.exc import IntegrityError
