# DatePicker

##Example
  
          var date = ""
          var time = ""
         
         
         SPicker.selectDate(title: "Select Date and Time", cancelText: "Cancel", datePickerMode: .dateAndTime, style: .Inline, didSelectDate: {[weak self] (selectedDate) in
            // TODO: Your implementation for date
            self?.date = selectedDate.dateString(format: "MM/dd/YYYY")
            self?.time = selectedDate.dateString(format: "hh:mm a")
            self?.dateTimeLable.text = selectedDate.dateString(format: "dd/MM/YYYY hh:mm a")
        })
