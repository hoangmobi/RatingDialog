# RatingDialog
Create simple rating dialog for application



 RatingDialog mRatingDialog = new RatingDialog(this);
 mRatingDialog.setRatingDialogListener(new RatingDialog.RatingDialogInterFace() {
            @Override
            public void onDismiss() {
                Log.v("RATELISTERNER","onDismiss ");
            }

            @Override
            public void onSubmit(float rating) {
                Log.v("RATELISTERNER","onSubmit "+rating);
            }

            @Override
            public void onRatingChanged(float rating) {
                Log.v("RATELISTERNER","onRatingChanged "+rating);
            }
        }); 




Call  mRatingDialog.showDialog(); in onBackPress to show dialog
Call  mRatingDialog.setEnable(boolean) to Disable/Emable show this next time
Call mRatingDialog.setDefaultRating(int rate) to set default rate
Call mRatingDialog.closeDialog() to dismiss dialog
