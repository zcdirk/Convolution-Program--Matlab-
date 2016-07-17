function varargout = juanji(varargin)
% JUANJI MATLAB code for juanji.fig
%      JUANJI, by itself, creates P new JUANJI or raises the existing
%      singleton*.
%
%      H = JUANJI returns the handle to P new JUANJI or the handle to
%      the existing singleton*.
%
%      JUANJI('CALLBACK',hObject,eventData,handles,...) calls the local
%      function named CALLBACK in JUANJI.M with the given input arguments.
%
%      JUANJI('Property','Value',...) creates P new JUANJI or raises the
%      existing singleton*.  Starting from the left, property value pairs are
%      applied to the GUI before juanji_OpeningFcn gets called.  An
%      unrecognized property name or invalid value makes property application
%      stop.  All inputs are passed to juanji_OpeningFcn via varargin.
%
%      *See GUI Options on GUIDE's Tools menu.  Choose "GUI allows only one
%      instance to run (singleton)".
%
% See also: GUIDE, GUIDATA, GUIHANDLES

% Edit the above text to modify the response to help juanji

% Last Modified by GUIDE v2.5 04-Dec-2013 13:12:44

% Begin initialization code - DO NOT EDIT
gui_Singleton = 1;
gui_State = struct('gui_Name',       mfilename, ...
                   'gui_Singleton',  gui_Singleton, ...
                   'gui_OpeningFcn', @juanji_OpeningFcn, ...
                   'gui_OutputFcn',  @juanji_OutputFcn, ...
                   'gui_LayoutFcn',  [] , ...
                   'gui_Callback',   []);
if nargin && ischar(varargin{1})
    gui_State.gui_Callback = str2func(varargin{1});
end

if nargout
    [varargout{1:nargout}] = gui_mainfcn(gui_State, varargin{:});
else
    gui_mainfcn(gui_State, varargin{:});
end
% End initialization code - DO NOT EDIT


% --- Executes during object creation, after setting all properties.
function P_CreateFcn(hObject, eventdata, handles)
% hObject    handle to P (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: place code in OpeningFcn to populate P



% --- Executes just before juanji is made visible.
function juanji_OpeningFcn(hObject, eventdata, handles, varargin)
% This function has no output args, see OutputFcn.
% hObject    handle to figure
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
% varargin   command line arguments to juanji (see VARARGIN)

% Choose default command line output for juanji
handles.output = hObject;

% Update handles structure
guidata(hObject, handles);

% UIWAIT makes juanji wait for user response (see UIRESUME)
% uiwait(handles.figure1);


% --- Outputs from this function are returned to the command line.
function varargout = juanji_OutputFcn(hObject, eventdata, handles) 
% varargout  cell array for returning output args (see VARARGOUT);
% hObject    handle to figure
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Get default command line output from handles structure
varargout{1} = handles.output;



function ys_Callback(hObject, eventdata, handles)
% hObject    handle to ys (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of ys as text
%        str2double(get(hObject,'String')) returns contents of ys as P double


% --- Executes during object creation, after setting all properties.
function ys_CreateFcn(hObject, eventdata, handles)
% hObject    handle to ys (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have P white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function yf_Callback(hObject, eventdata, handles)
% hObject    handle to yf (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of yf as text
%        str2double(get(hObject,'String')) returns contents of yf as P double


% --- Executes during object creation, after setting all properties.
function yf_CreateFcn(hObject, eventdata, handles)
% hObject    handle to yf (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have P white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function yh_Callback(hObject, eventdata, handles)
% hObject    handle to yh (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of yh as text
%        str2double(get(hObject,'String')) returns contents of yh as P double


% --- Executes during object creation, after setting all properties.
function yh_CreateFcn(hObject, eventdata, handles)
% hObject    handle to yh (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have P white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function xs_Callback(hObject, eventdata, handles)
% hObject    handle to xs (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of xs as text
%        str2double(get(hObject,'String')) returns contents of xs as P double


% --- Executes during object creation, after setting all properties.
function xs_CreateFcn(hObject, eventdata, handles)
% hObject    handle to xs (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have P white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function xf_Callback(hObject, eventdata, handles)
% hObject    handle to xf (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of xf as text
%        str2double(get(hObject,'String')) returns contents of xf as P double


% --- Executes during object creation, after setting all properties.
function xf_CreateFcn(hObject, eventdata, handles)
% hObject    handle to xf (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have P white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function xh_Callback(hObject, eventdata, handles)
% hObject    handle to xh (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of xh as text
%        str2double(get(hObject,'String')) returns contents of xh as P double


% --- Executes during object creation, after setting all properties.
function xh_CreateFcn(hObject, eventdata, handles)
% hObject    handle to xh (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have P white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end


% --- Executes on button press in create.
function create_Callback(hObject, eventdata, handles)
% hObject    handle to create (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
xs=str2double(get(handles.xs,'String'));
xf=str2double(get(handles.xf,'String'));
xh=str2double(get(handles.xh,'String'));
ys=str2double(get(handles.ys,'String'));
yf=str2double(get(handles.yf,'String'));
yh=str2double(get(handles.yh,'String'));
A=[-10 xs xs xf xf 10];
B=[0 0 xh xh 0 0];
C=[-10 ys ys yf yf 10];
D=[0 0 yh yh 0 0];
plot(handles.P,A,B,'-b',C,D,'-g');




% --- Executes on button press in start.
function start_Callback(hObject, eventdata, handles)
% hObject    handle to start (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
try
    delete(allchild(a));
    delete(allchild(b));
end
xs=str2double(get(handles.xs,'String'));
xf=str2double(get(handles.xf,'String'));
xh=str2double(get(handles.xh,'String'));
ys=str2double(get(handles.ys,'String'));
yf=str2double(get(handles.yf,'String'));
yh=str2double(get(handles.yh,'String'));
A=[-10 xs xs xf xf 10];
B=[0 0 xh xh 0 0];
C=[-10 -yf -yf -ys -ys 10];
D=[0 0 yh yh 0 0];
T=-10:0.02:10;
F=ones(size(T)).*and(T>=xs,T<=xf);
E=ones(size(T)).*and(T>=ys,T<=yf);
J=conv(E,F)*xh*yh/50;
T1=-20:0.02:20;
plot(handles.P,A,B,'-b',C,D,'-g');
pause(0.5)
for k=1:(xf+yf+5)*50;           
    pause(0.01);
    C=C+0.02;
    X=(T1<0.02*k)
    O=J.*X;
    plot(handles.P,A,B,'-b',C,D,'-g');
    plot(handles.Q,T1,O,'-r');
end


% --- Executes on button press in delete.
function delete_Callback(hObject, eventdata, handles)
% hObject    handle to delete (see GCBO)
% eventdata  reserved - to be defined in P future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
try
    delete(allchild(a));
    delete(allchild(b));
end


% --- Executes during object creation, after setting all properties.
function Q_CreateFcn(hObject, eventdata, handles)
% hObject    handle to Q (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: place code in OpeningFcn to populate Q
