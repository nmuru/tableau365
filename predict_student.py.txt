import pickle
def predict_student(model,X_test):
    model=pickle.load(open('dtmodel.sav','rb'))
    y_pred=model.predict(X_test)
    return y_pred